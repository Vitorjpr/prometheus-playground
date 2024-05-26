FROM golang AS buildando

WORKDIR /app
COPY . /app
RUN go build go_exporter.go
CMD ["./go_exporter"]

# FROM alpine:3.16
# COPY --from=buildando /app/go_exporter /app/go_exporter
# EXPOSE 7788
# WORKDIR /app
# CMD ["./go_exporter"]
