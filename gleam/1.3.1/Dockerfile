FROM ghcr.io/gleam-lang/gleam:v1.3.1-erlang-alpine

MAINTAINER "Cyteon"

RUN adduser --disabled-password --home /home/container container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ./entrypoint.sh /entrypoint.sh
CMD ["sh", "/entrypoint.sh"]
