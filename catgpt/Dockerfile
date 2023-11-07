FROM golang:1.21
WORKDIR /app
COPY . /app
RUN go mod download
RUN CGO_ENABLED=0 go build -o /godocker
EXPOSE 8080
CMD [ "/godocker" ]
