# PHP 5.4 with FPM and Magento dependencies
FROM debian:wheezy
MAINTAINER Abdullah <abdullah.rayeen@gmail.com>
RUN apt-get update -qqy && apt-get install -qqy php-soap php5 php5-curl php5-gd php5-mcrypt php5-mysql php5-xsl php5-xdebug php5-fpm php-apc
COPY php-fpm.conf /etc/php5/fpm/php-fpm.conf
COPY www-pool.conf /etc/php5/fpm/pool.d/www.conf
COPY xdebug-enabler.ini /etc/php5/fpm/conf.d/
CMD ["/usr/sbin/php5-fpm"]
EXPOSE 9001