FROM alpine:3.19
RUN apk update --no-cache
RUN apk upgrade --no-cache
RUN apk add openjdk17=17.0.12_p7-r0 --no-cache
RUN rm -rf /var/cache/apk/*
WORKDIR /app
COPY target/boot-swagger-4-0.0.1-SNAPSHOT.jar .
ENTRYPOINT sh -c 'java -jar *-SNAPSHOT.jar'
