# Specify base image
FROM node:16.17.0

WORKDIR /app

# Copy these files into image, then run npm install
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install --production

# Copies project directory into WORKDIR filesystem of the image
COPY . .

# The app binds to port 8080, use EXPOSE to map it
EXPOSE 8080

#  Run application
CMD [ "node", "index.js" ]