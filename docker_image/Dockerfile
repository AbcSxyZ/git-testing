FROM debian:bullseye-slim

ARG VERSION=2.0

RUN apt update && apt install -y wget

RUN wget https://github.com/dogecoin/dogecoin/releases/download/v1.14.5/dogecoin-1.14.5-i686-pc-linux-gnu.tar.gz

RUN echo build OK
