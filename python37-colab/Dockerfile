FROM python:3.7.6-slim-buster

RUN apt upgrade && apt install -y libjpeg8-dev zlib1g-dev libtiff-dev libfreetype6 libfreetype6-dev \
    libwebp-dev libopenjp2-7-dev libopenjp2-7-dev  && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ADD requirements.txt /var/projeto/requirements.txt

RUN pip install pipenv twine && pip install -r /var/projeto/requirements.txt 
