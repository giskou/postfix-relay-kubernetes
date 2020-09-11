FROM alpine:3.12.0

LABEL maintainer="ioannis.skoulis@confirmit.com"

RUN apk add --no-cache \
        postfix \
        rsyslog \
        supervisor && \
        /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/entrypoint.sh" ]
