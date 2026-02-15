FROM debian:trixie-slim

RUN apt-get update && apt-get install -y curl unzip

RUN curl -fsSL https://bun.sh/install | bash

ENV PATH="/root/.bun/bin:${PATH}"

WORKDIR /app
