FROM nginx:1.21.4-alpine
RUN rm -rf /usr/share/nginx/html/*
COPY build/ /usr/share/nginx/html
COPY config/nginx.conf etc/nginx/conf.d/
RUN sed -i '/access_log/c \    access_log \/dev\/null;server_tokens off;' /etc/nginx/nginx.conf
