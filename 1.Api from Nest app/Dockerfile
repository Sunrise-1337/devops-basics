FROM node:14-alpine AS build
WORKDIR /opt/app
COPY ./src/*.json .
RUN npm install
COPY ./src .
RUN npm run build api
CMD ["node", "./dist/apps/api/main.js"]