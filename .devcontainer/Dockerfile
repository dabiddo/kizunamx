FROM node:18.17-bookworm-slim 

WORKDIR /app

RUN apt update && \
    apt install git && \
    apt install openssh

RUN npm install -g pnpm

ENV HOST 0.0.0.0
EXPOSE 3000