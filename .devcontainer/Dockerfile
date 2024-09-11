FROM ruby:3.3.5

RUN apt-get update -y \
    && apt-get install -y libtool libffi-dev ruby-dev libzmq3-dev jupyter \
    && rm -rf /var/lib/apt/lists/*

RUN gem update --system && gem update

RUN gem install iruby && iruby register --force