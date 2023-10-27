FROM php:8.1-apache AS page

LABEL version=1.0

COPY /page /var/www/html

FROM nginx:1.24.0

COPY --from=page /var/www/html /usr/share/nginx/html

COPY /nginx /etc/nginx/conf.d/

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]

