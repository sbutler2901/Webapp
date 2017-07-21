# This file is designed to create a base docker images to be used for ReactJS
# 	it updates and installs git, nodejs, npm, vim, & go
FROM ubuntu:latest

RUN apt-get -y update

RUN apt-get install -y vim curl
RUN cd ~ && curl -O https://storage.googleapis.com/golang/go1.8.3.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf ~/go1.8.3.linux-amd64.tar.gz
RUN echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.profile
