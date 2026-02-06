# Command Executed

## Connect to database server
ssh peter@stdb01

## Switch to root user
sudo su

## Check MariaDB service status
systemctl status mariadb

## Restart MariaDB service
systemctl restart mariadb

## Check MariaDB service logs
journalctl -xeu mariadb.service

## Navigate to MariaDB data directory
cd /var/lib
ls -l

## Observation
mysql directory was missing

## Create mysql data directory
mkdir mysql

## Set correct ownership for MariaDB
chown -R mysql:mysql mysql

# Verification
systemctl restart mariadb
systemctl status mariadb
