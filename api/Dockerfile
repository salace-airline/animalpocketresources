# This Dockerfile assembles an image with all the dependencies required 
# to run golang from the command-line

# Build the Golang environment
FROM golang:1.20.2

WORKDIR /usr/src/app

RUN go install github.com/cosmtrek/air@latest

COPY . .
RUN go mod tidy
