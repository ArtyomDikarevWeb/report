FROM php:8.0-fpm

RUN apt-get update && \
      apt-get install curl && \
      apt-get install libcurl3-dev && \
      apt-get install libxml2-dev -y && \
      curl -sSL https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions -o - | sh -s \
      http intl mcrypt raphf redis ssh2 xsl yaml zip mysqli && \
      docker-php-ext-install curl pdo xml dom