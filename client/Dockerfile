FROM node:17-alpine

WORKDIR ./app

COPY package.json .

RUN npm i

RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache

COPY . .

EXPOSE 3000

CMD ["npm","start"]