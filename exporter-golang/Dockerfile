FROM golang:1.24-alpine3.21 AS builder

WORKDIR /app
COPY . /app

RUN go build segundo-exporter.go

FROM alpine:3.21

COPY --from=builder /app/segundo-exporter /app/segundo-exporter
EXPOSE 7788
WORKDIR /app
CMD ["./segundo-exporter"]

