# Docker-iti
examples of running commands of docker
# problem 2
Create react app docker container
```bash
    FROM ubuntu
    RUN apt-get update && apt-get install -y build-essential
    RUN apt-get install -y nodejs npm
    WORKDIR /app
    RUN npm install -g create-react-app
    RUN create-react-app react_app
    WORKDIR /app/react_app
    RUN npm install
    EXPOSE 3000
    CMD [ "npm","start" ]
```
