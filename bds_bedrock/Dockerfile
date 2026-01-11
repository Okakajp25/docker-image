FROM debian:trixie-slim

RUN apt-get update && apt-get install -y \
    libcurl4 \
    openssl \
    ca-certificates \
    curl \
    wget \
    unzip \
    tar \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /data

WORKDIR /data

ENV LD_LIBRARY_PATH=/date

EXPOSE 19132/udp
EXPOSE 19133/udp

CMD ["./bedrock_server"]
