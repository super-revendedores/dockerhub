FROM hashicorp/terraform:0.12.6

RUN apk add --update python py-pip openssl ca-certificates groff zip curl && \
    pip install --upgrade pip awscli && \
    rm -rf /var/cache/apk/*

ENTRYPOINT ["sh", "-c"]
