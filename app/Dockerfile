FROM php:7.1-fpm-alpine

ARG VERSION="2.18"

RUN apk add --no-cache libpng-dev curl-dev sqlite-dev

RUN docker-php-ext-install gd mbstring pdo_sqlite

RUN chown www-data:www-data /var/www/html

USER www-data

RUN echo "${VERSION}"

RUN wget "https://github.com/SSilence/selfoss/releases/download/${VERSION}/selfoss-${VERSION}.zip" \
    && unzip "selfoss-${VERSION}.zip" \
    && rm "selfoss-${VERSION}.zip"

VOLUME [ "/var/www/html" ]
