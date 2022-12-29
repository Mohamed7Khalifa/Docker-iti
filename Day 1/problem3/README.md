# Docker-iti
examples of running commands of docker
# create volume 
```bash
    sudo docker volume create [Volume_name]
```
# attach container to volume with port mapping
```bash 
    sudo docker run -it -v static_file:/var/www/html -p 8099:80 --name nginx-container nginx bash
```
# attach the same volume with another container
```bash 
    sudo docker run -it -v static_file:/var/www/html -p 8099:80 --name nginx-container1 nginx bash
```
<hr/>

