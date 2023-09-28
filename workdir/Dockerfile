FROM golang:1.18-alpine

ENV APP_PORT=8080

WORKDIR /app
COPY main.go /app

EXPOSE 8080

CMD go run main.go