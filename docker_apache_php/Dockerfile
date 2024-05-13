FROM php:apache

COPY apache-config.conf /etc/apache2/sites-available/000-default.conf

RUN a2enmod rewrite
RUN service apache2 restart

COPY . /var/www/html/
RUN chown -R www-data:www-data /var/www/html/
