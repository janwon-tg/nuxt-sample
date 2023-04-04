FROM node:19.8-bullseye

WORKDIR /usr/src/app

COPY package.json yarn.lock ./

RUN yarn

COPY . .

EXPOSE 8080

ENV HOST=0.0.0.0
ENV PORT=8080

RUN yarn install
CMD "yarn" "dev"
