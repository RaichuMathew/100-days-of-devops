# Commands Executed

## Connect to App server
ssh banner@stapp03

sudo su

## Create a docker network
docker network create -d bridge --subnet 192.168.30.0/24 --ip-range 192.168.30.0/24 media

## Verify the Configuration
docker network inspect media
