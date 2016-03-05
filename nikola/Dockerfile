FROM alpine:latest
MAINTAINER Gero Müller "post@geromueller.de"

RUN echo "@testing http://nl.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories
RUN apk add --update py-nikola@testing
RUN rm -rf /var/cache/apk/*
