FROM node:14.2-alpine

ENV TZ Asia/tokyo

RUN apk update \
  && apk add --update --no-cache --virtual=.build-dependencies g++

COPY --from=node /usr/local/bin /usr/local/bin
COPY --from=node /usr/local/lib /usr/local/lib
COPY --from=node /opt /opt

WORKDIR /app

CMD ["/bin/ash"]
