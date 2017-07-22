FROM alpine

ENV TESTCASE_BUILD_VERSION a1.0
ARG external_url
COPY www/* /var/www/localhost/htdocs/
COPY default.conf /etc/nginx/conf.d/default.conf 
RUN apk update && apk add nginx && mkdir -p /run/nginx

CMD ["nginx", "-g", "daemon off;"]
