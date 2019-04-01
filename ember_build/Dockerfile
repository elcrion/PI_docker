FROM node:8-slim

# For GOSU details see https://github.com/tianon/gosu/blob/master/INSTALL.md
RUN set -eux; \
    apt-get update; \
    apt-get install -y gosu \
        ca-certificates \
        gcc \
        git \
        build-essential \
        libssl-dev \
        libffi-dev \
        python \
        python-dev \
        git \
        python3-pip; \
    rm -rf /var/lib/apt/lists/*; \
    gosu nobody true; \
    apt-get clean; \
    update-ca-certificates; \
    npm -g install bower; \
    npm -g install ember-cli@3.8.1;

