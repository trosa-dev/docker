FROM node:18.17.0-alpine as builder

WORKDIR /app

COPY package.json .

RUN npm install --silent --cache --force

COPY . .

RUN npm install -g serve

RUN npm run build

CMD ["serve", "-s", "build"]

