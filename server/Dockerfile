FROM node:lts

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY .. /app

RUN npm build

EXPOSE 5000

CMD [ "node", "dist/main" ]