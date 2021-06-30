FROM php:7.4.5-alpine

RUN pecl install xdebug &&\
	docker-php-ext-enable xdebug

WORKDIR /src