FROM ruby:2.2.4

RUN apt-get update -yqq \
 && apt-get install -yqq --no-install-recommends \
    postgresql-client \
    nodejs \
 && apt-get -q clean \
 && rm -rf /var/lib/apt/lists
