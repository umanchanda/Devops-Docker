FROM golang:1.16

WORKDIR /go/src/app

COPY example-backend .

RUN go get -d -v ./...

RUN go install -v ./...

EXPOSE 8080

RUN go build

CMD ["./server"]