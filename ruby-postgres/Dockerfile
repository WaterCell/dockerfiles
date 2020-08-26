FROM ruby:2.7
RUN gem update --system && apt-get update -qq && \
    apt-get install -y -qq postgresql postgresql-contrib libpq-dev cmake && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
