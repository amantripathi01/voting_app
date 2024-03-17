FROM nginx:1.24-alpine3.17

COPY ./public/ /usr/share/nginx/html/

EXPOSE 80

CMD ["/bin/sh",  "-c",  "envsubst < /usr/share/nginx/html/environment/env.template.js > /usr/share/nginx/html/environment/env.js && exec nginx -g 'daemon off;'"]
