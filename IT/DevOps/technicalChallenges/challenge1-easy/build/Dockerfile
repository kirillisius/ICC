FROM alpine:latest

WORKDIR /app

COPY index.html /app/index.html

RUN apk add --no-cache thttpd

EXPOSE 80

CMD ["thttpd", "-D", "-h", "/app", "-p", "80"]

