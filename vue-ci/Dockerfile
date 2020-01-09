FROM node:12.14.1-alpine

RUN yarn global add @vue/cli @vue/cli-service @sentry/cli && \
    yarn cache clean --force

RUN apk -v --update add python3 curl && \
    python3 -m ensurepip  && \
    pip3 install awscli && \
    rm -rf /var/cache/apk/*
