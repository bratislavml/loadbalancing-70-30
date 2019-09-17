FROM golang:latest

RUN mkdir /app
ADD golang-webserver /app
WORKDIR /app

RUN ["chmod", "+x", "golang-webserver"]

CMD ["/app/golang-webserver"]