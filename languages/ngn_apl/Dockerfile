FROM registry.gitlab.pxeger.com/attempt-this-online/languages/node

ARG APL_REV=69fa5ba80f0ee846232e289934a9285da70a17ee

RUN curl -L https://github.com/abrudz/ngn-apl/archive/$APL_REV.tar.gz | \
    tar -xz && \
    mv ngn-apl-$APL_REV /opt/apl
