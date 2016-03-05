FROM debian:latest
MAINTAINER Gero Müller "post@geromueller.de"

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update
RUN apt-get install -y python3 python3-blinker python3-dateutil python3-docutils python3-doit python3-imaging python3-logbook python3-lxml python3-mako python3-natsort python3-pkg-resources python3-pygments python3-pyrss2gen python3-unidecode python3-yapsy
RUN apt-get autoclean
RUN apt-get clean
RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN pip3 install nikola
