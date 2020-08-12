FROM node:carbon

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY . /usr/src/app/
RUN npm install && npm run build

EXPOSE 80
ENTRYPOINT [ "npm", "start" ]
