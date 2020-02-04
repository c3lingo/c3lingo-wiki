FROM php:apache

RUN a2enmod rewrite

RUN apt-get update && apt-get install -y \
	msmtp \
 && rm -rf /var/lib/apt/lists/*

COPY msmtp.ini /usr/local/etc/php/conf.d/
