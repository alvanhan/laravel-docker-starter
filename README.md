# Docker Compose Laravel,Mysql,Nginx,Phpmyadmin
this is the starter template for docker compose laravel


## Usage
run this if using windows, in the src folder
```bash
docker run --rm -v ${PWD}:/app composer create-project --prefer-dist laravel/laravel /app
```

open docker and run 

```bash
#on your terminal
docker-compose build
docker-compose up -d
```
Run command
```bash
#on your terminal
docker exec -it php /bin/sh
chmod -R 777 storage
```
If app:key still empty on .env run php artisan key:generate on your terminal after going into the php container on docker
To run artisan commands like migrate, etc. go to php container using docker exec -it php /bin/sh


## 
