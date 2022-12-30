# Docker-iti
examples of running commands of docker
# problem 2
Create react app docker container in single stage
```bash
    FROM node:alpine3.16
    WORKDIR /app
    COPY package*.json ./
    RUN npm install
    COPY . .
    EXPOSE 3000
    CMD [ "npm","start" ]
```
Create react app docker container in multi stage
building stage
```bash
    FROM node:alpine3.16 AS build
    WORKDIR /app
    COPY package*.json ./
    RUN npm install
    COPY . .
    EXPOSE 3000
    RUN npm run build
```
deploy stage
building stage
```bash
    FROM nginx
    COPY --from=build /app/build /usr/share/nginx/html
    EXPOSE 80
    CMD [ "nginx", "-g", "daemon off;" ]
```
