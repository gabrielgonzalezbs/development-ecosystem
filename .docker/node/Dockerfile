FROM node:20.17.0-slim

RUN apt-get update && apt-get install -y openssl procps

WORKDIR /home/node/ecosystem

USER node

CMD tail -f /dev/null