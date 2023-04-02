FROM golang:1.20.1-alpine

WORKDIR /go/src/app
COPY ./app /go/src/app

RUN go install github.com/cosmtrek/air@latest
RUN go mod download

ENV CGO_ENABLED=0 \
    GOOS=linux \
    GOARCH=amd64

CMD ["air","-c",".air.toml"]

EXPOSE 3000
