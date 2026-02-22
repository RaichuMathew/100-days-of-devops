# Commands Executed

## Connect to app server 3
ssh banner@stapp03

sudo su

## Navigate to the repository and create the compose file
vi /opt/docker/docker-compose.yml

## Add Docker Compose Configuration

version: '3.8'

services:
  web_service :
  image : httpd:latest
  container_name: httpd
 ports:
  - "3000:80"
 volumes:
  - /opt/dba:/usr/local/apache2/htdocs
 restart: always
## Run the docker compse file
sudo docker compose up -d 
