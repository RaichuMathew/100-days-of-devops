# Day46:- Deploy an App on Docker Containers 

# Commands Executed

## Navigate to the repository

cd /opt/devops/

vi docker-compose.yml

## Add the below details in compose file


services:
  web:
    image: php:8.2-apache
    container_name: php_blog
    ports:
      - "8088:80"
    volumes:
      - "/var/www/html:/var/www/html"
    depends_on:
      - db

  db:
    image: mariadb:latest
    container_name: mysql_blog
    ports:
      - "3306:3306"
    volumes:
      - "/var/www/mysql:/var/lib/mysql"

    environment:
      MYSQL_DATABASE: database_blog
      MYSQL_USER: app_user
      MYSQL_PASSWORD: CompLex@P
      MYSQL_ROOT_PASSWORD: RootPas@*!


## Run the docker compose
docker compose up -d
