# This file is designed to create the docker image used to serve the ReactJS
#       webapp
FROM ubuntu:latest

RUN apt-get -y update

RUN apt-get install -y git nodejs npm vim

ADD init.sh /srv/
RUN chmod +x /srv/init.sh
#RUN /srv/init.sh

ADD start.sh /srv/
RUN chmod +x /srv/start.sh

ADD web_server.go /srv/

EXPOSE 8080

#CMD ["/bin/bash", "/srv/start.sh"]
