FROM ajaymakode/my-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY . .

RUN chmod +x capabilities.sh

ENTRYPOINT [ "/bin/sh","./capabilities.sh" ]
