FROM node:16-alpine

WORKDIR /usr/src/app

COPY package*.json ./

#RUN npm ci --only=production
RUN npm install
COPY . .

EXPOSE 8000

ENTRYPOINT node_modules/.bin/webpack-dev-server --config webpack.config.js --progress --inline --colors