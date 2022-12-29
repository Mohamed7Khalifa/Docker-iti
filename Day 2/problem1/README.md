# Docker-iti
examples of running commands of docker
# problem 1
P1: Create your own nginx docker image based on ubuntu “NEVER USE FROM nginx”
    • Install nginx
    • Two index.html one as file and another as .tar "/var/www/html"
    • Expose
    • Start
    • Port mapping
```bash
    FROM ubuntu
    RUN apt-get update
    RUN apt-get install nginx -y
    ADD index.html /var/www/html
    ADD index.tar /var/www/html
    EXPOSE 80
    CMD [ "nginx", "-g", "daemon off;" ]
```
```bash
    docker run -it -p 8080:80 my_nginx
```
# problem 2
# problem 3
# problem 4
