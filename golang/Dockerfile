FROM golang:1.16.5-alpine3.13 as builder
WORKDIR /app
COPY . /app
RUN CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -o server .

FROM scratch
COPY --from=builder /app/server /
EXPOSE 8080
CMD ["/server"]
