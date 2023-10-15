FROM node:18.17.0-alpine as builder

WORKDIR /app

COPY package.json .

RUN npm install --silent --cache --force

COPY . .

CMD ["npm", "start"]

