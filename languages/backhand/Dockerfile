FROM registry.gitlab.pxeger.com/attempt-this-online/languages/python

ARG BACKHAND_REV=8703a6d384005e18b0b87fd1360c241b9326ae07

RUN curl -L https://github.com/GrayJoKing/Backhand/archive/$BACKHAND_REV.tar.gz | \
    tar -xz && \
    mv Backhand-* /opt/backhand
