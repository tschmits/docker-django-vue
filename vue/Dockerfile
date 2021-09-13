# syntax=docker/dockerfile:1
FROM node:lts-alpine
ENV NODE_ENV=development
RUN yarn global add @vue/cli
COPY package.json yarn.lock /tmp/
RUN cd /tmp && yarn
WORKDIR /app
COPY . /app/
