# Version: 0.0.1
FROM ubuntu:14.04
MAINTAINER Dreammis "hysn2001@gmail.com"
ADD sources.list /etc/apt/

RUN apt-get update&&apt-get install -y nginx
RUN echo 'Hi, I am in your container' >/usr/share/nginx/html/index.html
# RUN touch /home/hello&&echo 'hi'> /home/hello
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
VOLUME ["/opt/project"]
EXPOSE 80
