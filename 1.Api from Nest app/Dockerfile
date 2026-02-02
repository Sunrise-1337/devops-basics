FROM node:14-alpine AS build
RUN apk add --no-cache git
WORKDIR /opt/app
RUN git clone https://github.com/AlariCode/docker-demo.git .
RUN npm install && npm run build api
CMD ["node", "./dist/apps/api/main.js"]