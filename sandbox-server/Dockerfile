FROM golang:1.11.1

ENV GO111MODULE=on
ENV GOPROXY=https://mirrors.aliyun.com/goproxy/
# ENV COMPOSE_CONVERT_WINDOWS_PATHS=1

# RUN mkdir /go/src/sandbox-server
# RUN chmod -R 777 /go/src/sandbox-server

WORKDIR /go/src/sandbox-server
COPY . .
RUN go get -u github.com/pilu/fresh
CMD ["fresh"]
EXPOSE 9999
