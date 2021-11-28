FROM ubuntu:bionic

WORKDIR /tmp/architecture

RUN apt update && apt install -y dpkg-dev
RUN dpkg --print-architecture #filter-tag-420
RUN dpkg-architecture --query DEB_BUILD_GNU_TYPE
RUN dpkg-architecture --query DEB_BUILD_MULTIARCH
RUN dpkg-architecture --query DEB_BUILD_ARCH
RUN uname -m

