FROM golang:1.16

WORKDIR /go/src/app
COPY example-backend .

EXPOSE 8080

RUN go get -d -v ./...
RUN go install -v ./...
RUN go build

ENV REQUEST_ORIGIN=localhost:8080

FROM node:14

WORKDIR /

COPY example-frontend .

EXPOSE 5000

RUN npm install && npm install -g serve
ENV REACT_APP_BACKEND_URL=localhost:5000
RUN npm run build

CMD [ "serve", "-s", "-l", "5000", "build" ]
