# syntax=docker/dockerfile:1

FROM node:12.18.1
ENV NODE_ENV=production

WORKDIR /app

RUN npm install --production

COPY ["package.json", "./"]
COPY ["package-lock.json*", "./"]

COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
