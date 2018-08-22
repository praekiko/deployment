FROM node:8.11.3-alpine

ARG APP_DIR=/app

RUN mkdir ${APP_DIR}
WORKDIR ${APP_DIR}

COPY package.json ${APP_DIR}
RUN npm install

COPY index.js ${APP_DIR}
COPY dist ${APP_DIR}/dist

EXPOSE 8080

CMD ["npm", "run", "start"]