FROM alpine:3.11

CMD [ "echo","Hello"]

FROM alpine:3.11

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY . .

RUN chmod +x run.sh

ENTRYPOINT [ "/bin/sh","./run.sh" ]