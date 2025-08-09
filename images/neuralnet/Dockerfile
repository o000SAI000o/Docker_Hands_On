FROM ubuntu:latest
LABEL "Author"="Vishwa"
LABEL "Project"="neural_network_static_web"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install apache2 git -y
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD neural.tar.gz /var/www/html
#COPY neural.tar.gz /var/www/html
