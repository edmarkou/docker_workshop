FROM alpine:latest

RUN set -x && \
  apk add --no-cache \
  python3 \
  groff \
  less \
  py-pip && \
  pip --no-cache-dir install awscli && \
  apk del py-pip && \
  adduser -D aws

ARG USER=aws

RUN adduser -D $USER

WORKDIR /home/$USER

USER $USER

CMD ["help"]

ENTRYPOINT ["aws"]