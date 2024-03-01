FROM golang:1.22

# copy app
ADD . /app
WORKDIR /app

# build
RUN go build -o build/gateway *.go

# server running port
EXPOSE 7654

ENTRYPOINT ["/app/docker-entrypoint.sh"]