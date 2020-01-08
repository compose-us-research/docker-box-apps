FROM alpine:latest
RUN apk update && apk add git nodejs npm
WORKDIR /pdf-document-feeder
RUN npm i -g pdf-document-feeder
WORKDIR /app
