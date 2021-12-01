FROM debian:bullseye-slim AS verify

RUN apt update && apt install -y wget

ARG VERSION=1.0

WORKDIR /tmp
RUN wget https://github.com/dogecoin/dogecoin/releases/download/v1.14.5/dogecoin-1.14.5-i686-pc-linux-gnu.tar.gz && \
    mv *.tar.gz dogecoin.tar.gz

RUN echo build OK

FROM ubuntu:bionic

WORKDIR /tmp

COPY --from=verify /tmp/dogecoin.tar.gz .

RUN ls

ENTRYPOINT ["/bin/sh"]
