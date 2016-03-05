FROM alpine:latest
MAINTAINER Gero Müller "post@geromueller.de"

RUN apk add --update python py-pip py-tz py-mako py-docutils py-unidecode py-lxml py-pillow py-pygments
RUN pip install nikola webassets
RUN rm -rf /var/cache/apk/*
