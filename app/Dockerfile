# syntax=docker/dockerfile:1

# Specify base image
FROM node:16.17.0

ENV NODE_ENV=production
WORKDIR /app

# Copy these files into image, then run npm install
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install --production

# Copies project directory into WORKDIR filesystem of the container
COPY . .

EXPOSE 3000

#  Run application
CMD [ "node", "index.js" ]