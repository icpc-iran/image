FROM ubuntu:22.04

WORKDIR /root/img/

COPY /etc/ssl/certs/ /etc/ssl/certs/
RUN sed -i 's|http://|https://|g' /etc/apt/sources.list # use https to don't allow university network to do man in the middle!
RUN apt update

ENTRYPOINT ./build.sh

