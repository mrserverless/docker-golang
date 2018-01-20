FROM golang:1.9-alpine

MAINTAINER Yun Zhi Lin <yun@yunspace.com>

RUN apk add --no-cache --update git openssh ca-certificates curl make bash g++ \
  && update-ca-certificates \
  && rm -rf /var/cache/apk/*

RUN go get -u github.com/golang/dep/cmd/dep

CMD [ "dep", "version" ]