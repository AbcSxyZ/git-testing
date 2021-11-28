FROM ubuntu:bionic

WORKDIR /tmp/architecture

RUN apt update && apt install -y dpkg-dev
RUN dpkg --print-architecture > arch1
RUN dpkg-architecture --query DEB_BUILD_GNU_TYPE > arch2
RUN dpkg-architecture --query DEB_BUILD_MULTIARCH > arch3
RUN dpkg-architecture --query DEB_BUILD_ARCH > arch4
RUN uname -m > arch5

