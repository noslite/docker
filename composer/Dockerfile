FROM php:7.1-alpine
RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
    php composer-setup.php --install-dir=/usr/bin --filename=composer  && \
    php -r "unlink('composer-setup.php');"
WORKDIR /var/www/noslite
ENTRYPOINT ["/usr/bin/composer"]
