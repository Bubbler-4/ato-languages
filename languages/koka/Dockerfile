FROM registry.gitlab.pxeger.com/attempt-this-online/languages/base

ARG KOKA_VERSION=2.4.2

RUN pacman -Syu --noconfirm cmake ninja && \
    mkdir /opt/koka && \
    curl -L https://github.com/koka-lang/koka/releases/download/v$KOKA_VERSION/koka-v$KOKA_VERSION-linux-x64.tar.gz | \
    tar -xzC /opt/koka && \
    ln -s /opt/koka/bin/koka /usr/local/bin/koka
