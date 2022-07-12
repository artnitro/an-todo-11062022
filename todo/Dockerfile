FROM nginx:alpine

RUN adduser -D -g 'www' www
RUN mkdir /www
RUN chown -R www:www /usr/share/nginx
RUN chown -R www:www /www

COPY ./proxy.conf /etc/nginx/proxy.conf 
COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./certs/. /etc/nginx/.
