# syntax=docker/dockerfile:1

FROM node:16.17.0

ENV NODE_ENV=production
WORKDIR /app

# Before running npm i, copy these files into images
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install --production

COPY . .

CMD [ "node", "index.js" ]