FROM php:7.4.5-alpine

RUN apk add --no-cache gcc g++ make autoconf

RUN pecl install xdebug &&\
	docker-php-ext-enable xdebug

WORKDIR /src