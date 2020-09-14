FROM alpine:3.12.0

LABEL maintainer="ioannis.skoulis@confirmit.com"

RUN apk add --no-cache \
        cyrus-sasl \
        cyrus-sasl-plain \
        postfix \
        rsyslog \
        supervisor && \
        /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/entrypoint.sh" ]
