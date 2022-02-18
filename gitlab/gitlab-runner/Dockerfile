FROM alpine:3.15

MAINTAINER gotoeasy <gotoeasy@163.com>

RUN apk add --no-cache curl \
 && curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/v11.1.0/binaries/gitlab-runner-linux-amd64" \
 && chmod +x /usr/local/bin/gitlab-runner \
 && apk del curl \
 && rm /var/cache/apk/*

# 版本查看
# https://gitlab.com/gitlab-org/gitlab-runner/-/tags
# 直接下载另存为
# curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/v11.1.0/binaries/gitlab-runner-linux-amd64"
