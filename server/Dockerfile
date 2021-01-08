FROM golang:1.14-alpine
LABEL MAINTAINER casio.pro

ENV GO111MODULE=on

WORKDIR /go/src/
COPY . .

RUN apk update && \
    apk add --no-cache git

RUN go get -u github.com/360EntSecGroup-Skylar/excelize \
    github.com/BurntSushi/toml \
    github.com/labstack/echo/middleware