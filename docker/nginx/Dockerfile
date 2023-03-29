FROM nginx:1.20-alpine

ENV TZ Asia/Tokyo

COPY ./docker/nginx/default.conf /etc/nginx/conf.d/default.conf

RUN apk update && \
    apk add tree && \
    apk add vim