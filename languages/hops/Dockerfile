FROM registry.gitlab.pxeger.com/attempt-this-online/languages/haskell

ARG HOPS_REV=fa5c0c731d586a50b86d2b0c08350d53769295e9

COPY without_doc.patch /tmp/

RUN curl -L https://github.com/akc/hops/archive/$HOPS_REV.tar.gz | \
    tar -xz && \
    cd hops-$HOPS_REV && \
    patch < /tmp/without_doc.patch && \
    rm /tmp/without_doc.patch && \
    cabal --store-dir /opt/cabal install --package-env /opt/ghc_env --install-method=copy --installdir /usr/local/bin --allow-newer && \
    cd / && \
    rm -rf /tmp/hops-$HOPS_REV
