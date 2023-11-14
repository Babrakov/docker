###

FROM ubuntu:18.04

RUN apt -y update
RUN apt -y install apache2

RUN echo 'Hello World' > /var/www/html/index.html

CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]
EXPOSE  80