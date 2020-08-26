FROM node:8.17.0-slim
RUN apt-get update -qq && \
    apt-get install -y ocaml libelf-dev && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
