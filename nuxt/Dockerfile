FROM node:10.11.0-alpine

RUN apk update && apk upgrade

RUN mkdir -p /app
WORKDIR /app

COPY . /app
RUN npm install

RUN npm run build

ENV HOST 0.0.0.0
EXPOSE 3000

CMD ["npm", "start"]
