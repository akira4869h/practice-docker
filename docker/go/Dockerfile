FROM ubuntu:22.04

RUN apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install -y \
        wget \
        curl \
        vim \
        git \
        tar \
        build-essential \
        zlib1g-dev \
        libssl-dev \
        libyaml-dev \
        libreadline-dev

RUN wget https://go.dev/dl/go1.21.3.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go1.21.3.linux-amd64.tar.gz && \
    rm go1.21.3.linux-amd64.tar.gz

ENV PATH=$PATH:/usr/local/go/bin