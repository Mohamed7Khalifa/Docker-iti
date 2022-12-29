# Docker-iti
examples of running commands of docker
# install container without attach to volume
```bash 
    sudo docker run -it  -p 8099:80 --name nginx-container1 nginx bash
```
# Commit the container with image name my apache
```bash 
    sudo docker commit 718f
```
# Create a dockerfile for ngnix and build the image from this dockerfile
```bash
    sudo docker build .
```



