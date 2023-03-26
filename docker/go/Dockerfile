FROM golang:latest

WORKDIR /go/src/app
COPY ./app /go/src/app

ENV CGO_ENABLED=0 \
    GOOS=linux \
    GOARCH=amd64
EXPOSE 3000
