FROM php:5.6-apache
 
# Install PDO MySQL driver
# See https://github.com/docker-library/php/issues/62
RUN docker-php-ext-install pdo mysql
RUN docker-php-ext-install pdo mysqli
RUN mkdir /var/www/html/data
RUN apt-get update
RUN apt-get install -y git
RUN git clone https://github.com/MohamedKaraga/Cloud.git /var/www/html/data
