FROM node:14.2-alpine

ENV TZ Asia/tokyo

RUN apk update \
  && apk add --update --no-cache --virtual=.build-dependencies g++ && \
  apk add --no-cache curl && \
  curl -o- -L https://yarnpkg.com/install.sh | sh

WORKDIR /app

CMD ["/bin/ash"]
