FROM node:14.5.0-slim

RUN apt-get update \
  && apt-get -y install curl unzip gzip git locales\
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /build
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
  && unzip awscliv2.zip \
  && ./aws/install \
  && rm -rf aws awscliv2.zip

ENV TZ Asia/Tokyo

WORKDIR /work