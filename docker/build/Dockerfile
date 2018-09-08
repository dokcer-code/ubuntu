FROM ubuntu:18.04
RUN apt-get update && apt-get install -y apt-utils curl gnupg less

# nginx
RUN curl http://nginx.org/keys/nginx_signing.key | apt-key add -
RUN echo "deb http://nginx.org/packages/ubuntu/ bionic nginx" >> /etc/apt/sources.list
RUN echo "deb-src http://nginx.org/packages/ubuntu/ bionic nginx" >> /etc/apt/sources.list
RUN apt-get update && apt-get install -y nginx
CMD nginx