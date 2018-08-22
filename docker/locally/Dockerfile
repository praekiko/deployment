FROM node:8.11.3-alpine

ARG APP_DIR=/app

RUN mkdir ${APP_DIR}
WORKDIR ${APP_DIR}

COPY package.json ${APP_DIR}
RUN npm install

COPY src ${APP_DIR}/src
COPY index.js ${APP_DIR}

EXPOSE 8080

RUN npm run build

CMD ["npm", "run", "start"]