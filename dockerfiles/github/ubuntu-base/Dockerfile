FROM ubuntu:latest
MAINTAINER Gissehel <public-docker-github-ubuntu-base-maintainer@gissehel.org>

ARG BUILD_DATE
ARG VCS_REF

LABEL \
      org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.name=ubuntu-base \
      org.label-schema.version=1.21-$VCS_REF \
      org.label-schema.vendor=gissehel \
      org.label-schema.vcs-url="https://github.com/gissehel/docker-gissehel-images" \
      org.label-schema.schema-version="1.0"

ADD script.sh /tmp/create-image-script
RUN /bin/bash /tmp/create-image-script && rm -f /tmp/create-image-script

