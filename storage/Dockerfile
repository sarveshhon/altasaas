FROM golang:1.22

# copy app
ADD . /app
WORKDIR /app

# build
RUN go build -o build/storage *.go

# server running port
EXPOSE 7654

RUN chmod +x /app/docker-entrypoint.sh
ENTRYPOINT ["/app/docker-entrypoint.sh"]