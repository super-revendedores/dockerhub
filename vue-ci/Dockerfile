FROM node:12.13.0-alpine

RUN yarn global add @vue/cli @vue/cli-service @sentry/cli

RUN apk -v --update add python3 && \
    python3 -m ensurepip  && \
    pip3 install awscli
