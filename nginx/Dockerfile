FROM nginx:alpine

COPY default.conf /etc/nginx/conf.d/default.conf

RUN apk --no-cache add tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata

RUN apk add --no-cache certbot