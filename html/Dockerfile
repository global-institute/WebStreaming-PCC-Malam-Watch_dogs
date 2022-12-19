FROM ubuntu 
RUN apt update 
RUN apt upgrade
RUN apt-get install -y apache2 
RUN apt-get install -y apache2-utils 
RUN apt clean 
COPY ./html/. /var/www/html
WORKDIR /var/www/html
CMD ["apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80 443