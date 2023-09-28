FROM golang:1.18-alpine as builder

WORKDIR /app/
COPY main.go /app/
RUN go build -o /app/main /app/main.go
EXPOSE 8080

FROM alpine:3

WORKDIR /app/
COPY --from=builder /app/main /app/
CMD /app/main