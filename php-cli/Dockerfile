FROM php:7.1-alpine
RUN crontab -l | { cat; echo "* * * * * php /var/www/noslite/src/noslite.php"; } | crontab -
WORKDIR /var/www/noslite
RUN apk update && \
    apk upgrade && \
    apk add --update tzdata && \
    cp /usr/share/zoneinfo/Europe/Amsterdam /etc/localtime && \
    echo "Europe/Amsterdam" > /etc/timezone
RUN php src/noslite.php
CMD ["crond", "-f"]
