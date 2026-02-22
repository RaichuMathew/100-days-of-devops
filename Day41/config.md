# Commands Executed 
## Connect to App server 3
ssh banner@stapp03

sudo su

## Navigate to repository
cd /opt/docker

## Create Docker file

vi Dockerfile

FROM ubuntu:24.04
RUN apt update && apt install apache2 -y && sed -i 's/Listen 80/Listen 8084/' /etc/apache2/ports.conf

CMD ["usr/sbin/apache2ctl", "-D", "FOREGROUND"]

## Execute docker run command
docker build -t test .

docker run -d -p 90:8084 test

# Verification 
curl stapp03:90
