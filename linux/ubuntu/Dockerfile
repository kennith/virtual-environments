FROM ubuntu:18.04

RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get -yq update            && \
    apt-get install -yq tzdata    && \
    apt-get install -yq git       && \
    apt-get install -yq awscli    && \
    apt-get install -yq apache2   && \
    apt-get install -yq php
RUN /etc/init.d/apache2 restart