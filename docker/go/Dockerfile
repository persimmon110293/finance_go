FROM golang:latest

COPY ./app ./src/app

ENV CGO_ENABLED=0 \
    GOOS=linux \
    GOARCH=amd64
EXPOSE 3000
