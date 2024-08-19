FROM node:20-alpine

RUN addgroup app && adduser -S -G app app

USER app

WORKDIR /app 

COPY package*.json .

RUN yarn

COPY . .

EXPOSE 8000

CMD [ "yarn","start" ]