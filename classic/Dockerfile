FROM trafex/php-nginx:2.2.0


WORKDIR /var/www/html

RUN apk update && \
    apk -y install --no-install-recommends \
    apt-utils \
    unzip \
    libfreetype6-dev \
    libjpeg62-turbo-dev \
    libmcrypt-dev \
    libpng-dev \
    libmemcached-dev \
    zlib1g-dev \
    imagemagick

RUN wget https://github.com/omeka/Omeka/releases/download/v3.0.2/omeka-3.0.2.zip
RUN unzip omeka-3.0.2.zip


#Install php-extensions
#RUN pecl install mcrypt-1.0.3
#RUN docker-php-ext-enable mcrypt
#RUN docker-php-ext-install -j$(nproc) iconv pdo pdo_mysql gd mysqli
#RUN docker-php-ext-configure gd --with-freetype=/usr/include/ --with-jpeg=/usr/include/


