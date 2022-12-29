# Docker-iti
examples of running commands of docker
# problem 4
create ur own user-defined network
```bash
    docker network create my_network
```
create ur first machine and assign it to ur user-defined network
```bash
    docker run -it --name machine_one --network my_network ubuntu
```
create ur first machine and assign it to ur user-defined network
```bash
    docker run -it --name machine_two --network my_network ubuntu
```
install ping command cause docker image are pretty minimal
```bash
    apt-get update -y
    apt-get install -y iputils-ping
```
ping in the another machine by name 
```bash
    ping machine_one
```