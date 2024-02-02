FROM php:8.2-fpm

RUN apt-get -y update && apt-get install -y \
    libicu-dev \
    gcc \
    curl \
    libcurl4 \
    libcurl4-openssl-dev \
    zip \
    unzip \
    git \
    zlib1g-dev \
    libfreetype-dev \
    libjpeg62-turbo-dev \
    libpng-dev \
    icu-devtools \
    gettext \
    locales \
    build-essential \
    libxml2-dev \
    libzip-dev \
    libonig-dev
RUN docker-php-ext-install pdo pdo_pgsql pgsql intl mbstring simplexml xmlwriter zip gd gettext curl
RUN docker-php-ext-enable pgsql mbstring curl intl gd gettext simplexml xmlwriter zip