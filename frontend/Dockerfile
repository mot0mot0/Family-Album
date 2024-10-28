FROM node:20

WORKDIR /app

COPY frontend/package.json frontend/yarn.lock ./

RUN yarn install

COPY frontend ./

RUN yarn build

EXPOSE 3000

CMD ["yarn", "run", "dev"]
