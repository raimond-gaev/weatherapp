FROM node:19-alpine
LABEL org.opencointainers.image.source=https://github.com/raimond-gaev/test-repo
WORKDIR /usr/src/app
ENV APPID=c1aca0f4e7d72097ea5bd7895e545601
COPY package*.json ./

RUN npm ci --only=production

COPY . .

EXPOSE 9000

CMD ["node", "src/index.js"]