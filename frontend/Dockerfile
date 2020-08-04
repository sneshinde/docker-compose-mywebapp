FROM centos:7
MAINTAINER snehalshinde2112@gmail.com
RUN yum -y update
RUN yum -y install httpd php php-gd php-mysql
ADD code /var/www/html/
ENV MY_DB_HOST_WRITE=test MY_DB_HOST_READ=test MY_DB_NAME=test MY_DB_USER=test MY_DB_PASS=test
EXPOSE 80
LABEL appname=myapp
CMD ["httpd", "-D", "FOREGROUND"]