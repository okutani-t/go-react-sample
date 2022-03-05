FROM golang:1.17.7-alpine

RUN apk update
RUN apk add git

ENV ROOT=/go/src/app
WORKDIR ${ROOT}

COPY ./api/main.go ${ROOT}

EXPOSE 8080

ENTRYPOINT ["go", "run", "main.go"]
