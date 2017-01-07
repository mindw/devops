FROM alpine:3.5
MAINTAINER Gabi Davar <grizzly.nyo@gmail.com>

ENV PACKAGES "curl openssl ca-certificates groff less python3"

RUN apk --no-cache add $PACKAGES \
    && pip3 --no-cache-dir --disable-pip-version-check install --no-compile -U pip setuptools \
    && find / \( -name \*.pyc -o -name \*.pyo -o -name __pycache__ \) -prune -exec rm -rf {} +
    
