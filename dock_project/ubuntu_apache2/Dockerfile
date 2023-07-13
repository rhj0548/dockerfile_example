FROM ubuntu:focal
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y apache2 git
RUN git clone https://github.com/rhj0548/static-web-template.git 
RUN cp -r static-web-template/htdocs/* /var/www/html/
CMD ["apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
