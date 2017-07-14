FROM debian:sid

COPY sources.list /etc/apt/sources.list

RUN \
    apt-get update && \
    env DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends apt-utils && \
    env DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y && \
    env DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends build-essential && \
    apt-get clean

