FROM nginx:latest
MAINTAINER Vinh Le <hung.vjnh@gmail.com>

ENV www_path /home/vinhlh/vinh.ninja

RUN apt-get update && apt-get install -y git
RUN mkdir -p $www_path && git clone https://github.com/vinhlh/vinh.ninja.git $www_path
COPY configs/nginx.conf /etc/nginx/nginx.conf
