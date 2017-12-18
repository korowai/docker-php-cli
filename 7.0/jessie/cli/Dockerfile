#
# NOTE: FILE GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY
#
FROM php:7.0-cli-jessie
MAINTAINER Paweł Tomulik <ptomulik@meil.pw.edu.pl>

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
      libldap2-dev \
      libsasl2-dev && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* && \
    docker-php-ext-configure ldap --with-libdir=lib/x86_64-linux-gnu --with-ldap-sasl && \
    docker-php-ext-install ldap

# vim: set ft=dockerfile:
