FROM ubuntu:focal
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y nginx git
RUN git clone https://github.com/rhj0548/static-web-template.git
RUN cp -r static-web-template/htdocs/* /var/www/html/
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80
