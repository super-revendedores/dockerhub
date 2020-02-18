FROM python:3.7.6-alpine3.11

RUN apk upgrade && apk add --no-cache --virtual build-dependencies linux-headers make gcc g++ jq curl \
    postgresql-dev mariadb-dev unixodbc-dev ca-certificates zlib-dev jpeg-dev tiff-dev freetype-dev libc-dev lcms2-dev libwebp-dev \
    tcl-dev tk-dev libxml2-dev libxslt-dev && rm -rf /var/cache/apk/*

ADD requirements.txt /var/projeto/requirements.txt

RUN pip install pipenv twine && pip install -r /var/projeto/requirements.txt 
