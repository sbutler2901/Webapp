# This file is designed to create a base nginx server needed to act as a reverse proxy
#       to the ReactJS nodes
FROM ubuntu:latest

MAINTAINER sbutler

RUN apt-get -y update

RUN apt-get install -y vim nginx

RUN rm -v /etc/nginx/nginx.conf

ADD nginx.conf /etc/nginx/

#EXPOSE 80

CMD service nginx start
