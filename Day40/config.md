# Command Executed
## Connect to app server
ssh banner@stapp03

sudo su

## Navigating to container
docker exec -it c5359cc06064 bash

## Installing apache2
apt update

apt install apache2 -y

apt instal vim
## Updating the port 
sed -i 's|Listen 80|Listen 8085|' /etc/apache2/ports.conf

## Starting apache 2
service apache2 start

service apache2 status

