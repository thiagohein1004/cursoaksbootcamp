FROM node:12-alpine

RUN mkdir -p /usr/src/app
COPY ["./package.json", "./package-lock.json", "./src", "./tsconfig.json", "/usr/src/app/"]
WORKDIR /usr/src/app

RUN npm install && npm run build
EXPOSE 3000

ENTRYPOINT [ "npm", "start" ]
