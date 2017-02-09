FROM nginx:1.10.3

COPY ./default.conf /etc/nginx/conf.d/default.conf

RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

VOLUME /var/www

EXPOSE 80

EXPOSE 443
