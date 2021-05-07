### Dockerfile
FROM alpine:3.13.1

LABEL Author="Fatorin"
LABEL version="1.2"
LABEL description="Support for Warcraft III 1.28f."

# RUN echo -e "http://dl-cdn.alpinelinux.org/alpine/v3.13/main" > /etc/apk/repositories
RUN apk add alpine-baselayout mariadb-connector-c-dev boost-thread boost-filesystem libbz2 gmp libstdc++

# Set the working directory to /app
WORKDIR /app

RUN mkdir config
RUN mkdir maps

ADD ghostpp.tar /app
ADD include.tar /usr/local
ADD lib.tar /usr/local

CMD [ "ghost++" ]