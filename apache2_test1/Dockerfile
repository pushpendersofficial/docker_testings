FROM ubuntu:16.04
RUN apt-get update && apt install -y apache2 && apt-get clean && rm -rf /var/lib/apt/list/* 

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

EXPOSE 80

CMD ["apachectl", "-D", "FOREGROUND"]
