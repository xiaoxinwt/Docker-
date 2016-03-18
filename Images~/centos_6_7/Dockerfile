FROM centos:6.7
MAINTAINER xiaoxinwt "xiaoxinwt@163.com"
RUN yum -y update
RUN yum install -y httpd
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache
ONBUILD ADD . /var/www/
EXPOSE 80
ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D","FOREGROUND"]

