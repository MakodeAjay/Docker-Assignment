FROM alpine:3.11 as builder

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY /usr/src/app .
RUN echo ${Hello}

FROM builder
WORKDIR /usr/src/app
COPY --from=builder /usr/src/app .
RUN chmod +x run.sh
ENTRYPOINT [ "/bin/sh","./run.sh" ]

