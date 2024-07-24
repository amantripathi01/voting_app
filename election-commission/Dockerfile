FROM nginx:1.26.1-alpine3.19

COPY ./public/ /usr/share/nginx/html/

EXPOSE 80

CMD ["/bin/sh",  "-c",  "envsubst < /usr/share/nginx/html/environment/env.template.js > /usr/share/nginx/html/environment/env.js && exec nginx -g 'daemon off;'"]
