FROM nginx:alpine

RUN apk -U upgrade

RUN apk --no-cache add tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata

COPY default.conf /etc/nginx/conf.d/default.conf