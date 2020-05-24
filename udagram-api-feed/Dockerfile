# Nodejs image
FROM node:12

# Create app directory
WORKDIR /usr/src/app

# package.json AND package-lock.json are copied
COPY package*.json ./

# Install app dependencies
RUN npm ci

COPY . .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]