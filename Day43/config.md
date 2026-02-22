# Commands Executed

## Connect to App server 3
ssh banner@stapp03

sudo su

## Pull docker image
docker pull nginx:alpine-perl

## Create docker container
docker run -d -p 5003:80 --name cluster nginx:alpine-perl
