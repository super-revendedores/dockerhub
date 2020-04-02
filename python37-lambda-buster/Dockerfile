FROM python:3.7.7-slim-buster

RUN apt-get update \
 && apt-get install gcc curl wget -y \
 && curl -sL https://deb.nodesource.com/setup_12.x | sudo bash - \
 && apt-get install nodejs -y \
 && npm install yarn @sentry/cli -g --unsafe-perm \
 && pip install pipenv awscli \
 && apt-get clean \
 && yarn cache clean


