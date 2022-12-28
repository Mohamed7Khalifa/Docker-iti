### Docker-iti
examples of running commands of docker
# to run ubuntu container in interactive mode
first pull and run ubuntu image
```bash
    sudo docker pull ubuntu
```
run this image
```bash
    sudo docker run ubuntu
```
# To access the interactive mode
```bash
    sudo docker run -it ubuntu
```
run echo docker command
```bash
    root@4710be6d4ad6:/# echo docker
```
the output of this command --> docker
create file with name hello-docker
```bash
    root@4710be6d4ad6:/# touch hello-docker
```
to stop ubuntu container 
```bash
    root@4710be6d4ad6:/# exit
```
or press Ctrl+c
to remove ubuntu container
```bash
    sudo docker rm [container_id]
```
and this will remove the file also