  
FROM python:3.7.5-alpine3.10

RUN apk upgrade && apk add --no-cache --virtual build-dependencies linux-headers make gcc g++ jq \
    postgresql-dev mariadb-dev unixodbc-dev ca-certificates zlib-dev jpeg-dev tiff-dev freetype-dev libc-dev lcms2-dev libwebp-dev \
    libffi-dev tcl-dev tk-dev libxml2-dev libxslt-dev nodejs nodejs-npm bash curl && rm -rf /var/cache/apk/*
    
RUN npm install -g @sentry/cli --unsafe-perm

RUN pip install pipenv awscli
