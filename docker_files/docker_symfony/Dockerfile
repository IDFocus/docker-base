FROM phpdockerio/php:8.2-fpm
WORKDIR "/application/"

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php8.2-mysql \
    && apt-get -y install php8.2-soap \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

# Install git and update
RUN apt-get update \
    && apt-get -y install git \
&& apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
