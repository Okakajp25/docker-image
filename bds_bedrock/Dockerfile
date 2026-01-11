FROM debian:bookworm-slim

RUN apt-get update && apt-get install -y \
    libcurl4 \
    openssl \
    ca-certificates \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /data

WORKDIR /data

ENV LD_LIBRARY_PATH=.

EXPOSE 19133/udp
EXPOSE 19134/udp

CMD ["./bedrock_server"]
