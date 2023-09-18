FROM php:7.4-cli-alpine
FROM yiisoftware/yii2-php:7.4-fpm-nginx
ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/
ADD /project/yii-server/ /app/
RUN chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions redis