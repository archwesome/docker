FROM ubuntu:12.04
MAINTAINER Cristia Benitez Alvarez "lartex7@gmail.com"
RUN apt-get update
RUN apt-get install -y nginx
VOLUME /usr/share/nginx/www/
ARG webpage
ADD $webpage /usr/share/nginx/www/
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
EXPOSE 80
