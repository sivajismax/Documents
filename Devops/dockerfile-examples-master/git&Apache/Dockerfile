# A basic apache server. To use either add or bind mount content under /var/www
FROM centos

MAINTAINER MAHESH

RUN yum update && yum install -y apache2
RUN yum install git && yum install java

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

EXPOSE 80

CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
