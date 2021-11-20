FROM debian:latest

RUN apt update && apt install -y  --fix-broken dpkg-dev

RUN dpkg-architecture --query DEB_BUILD_GNU_TYPE > /architecture

ENTRYPOINT ["bash"]
