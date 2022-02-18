FROM alpine:3.15

MAINTAINER gotoeasy <gotoeasy@163.com>

RUN apk add --update -t curl \
 && curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/v11.1.0/binaries/gitlab-runner-linux-amd64" \
 && chmod +x /usr/local/bin/gitlab-runner \
 && apk del --purge deps \
 && rm /var/cache/apk/*
