# Docker-iti
examples of running commands of docker
```bash
    sudo docker run -d -p 3000:3306 -e MYSQL_ROOT_PASSWORD="P4sSw0rd0!" -v mysql_data:/var/lib/mysql  --name app-database mysql
```