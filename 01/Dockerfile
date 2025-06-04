FROM golang:1.24-alpine3.22 AS builder

COPY main.go .
WORKDIR / 
RUN go build main.go

CMD ["./main"]

COPY --from=builder /main /