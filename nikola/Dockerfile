FROM debian:latest
MAINTAINER Gero Müller "post@geromueller.de"

RUN DEBIAN_FRONTEND=noninteractive apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install locales
RUN echo -e "en_US.UTF-8 UTF-8\nde_DE.UTF-8 UTF-8" > /etc/locale.gen
RUN locale-gen
RUN DEBIAN_FRONTEND=noninteractive apt-get install --no-install-recommends  -y python3 python3-pip python3-blinker python3-dateutil python3-docutils python3-doit python3-pil python3-logbook python3-lxml python3-mako python3-natsort python3-pkg-resources python3-pygments python3-pyrss2gen python3-unidecode python3-yapsy
RUN DEBIAN_FRONTEND=noninteractive apt-get autoclean
RUN DEBIAN_FRONTEND=noninteractive apt-get clean
RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN pip3 install nikola
