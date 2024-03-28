FROM ubuntu:latest
RUN apt update && apt upgrade -y
RUN apt install apache2 -y
RUN service apache2 start
RUN apt install default-jdk -y
COPY index.html /var/www/html
EXPOSE 8002
#Start apache service in container
CMD apachectl -D FOREGROUND  