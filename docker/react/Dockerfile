FROM node:16-alpine

ENV ROOT=/app/react
WORKDIR ${ROOT}

COPY ./front/package.json .
COPY ./front/yarn.lock .

RUN yarn install

COPY ./front .

ENTRYPOINT [ "yarn", "start" ]
