FROM ruby:2.2.4

RUN apt-get update -yqq \
 && apt-get install -yqq --no-install-recommends \
    postgresql-client \
    nodejs \
 && apt-get -q clean \
 && rm -rf /var/lib/apt/lists

RUN gem install nokogiri -v "1.6.8.1"

ADD Gemfile* /var/app/
RUN cd /var/app && bundle install --without development test
