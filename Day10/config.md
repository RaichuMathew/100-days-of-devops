# Command Executed

## Connect to App Server 3
ssh banner@stapp03

## Install zip package (pre-requisite)
yum install zip -y

## Navigate to the scripts directory
cd /scripts

## Create backup script
vi beta_backup.sh
## Add the below in the scrip
!#/bin/bash
zip /backup/xfusioncorp_beta.zip /var/www/html/beta
scp /backup/xfusioncorp_beta.zip clint@stbkp01:/backup

## Make script executable
chmod +x beta_backup.sh

## Configure passwordless SSH to Nautilus Backup Server
ssh-keygen -t rsa
ssh-copy-id clint@stbkp01
Enter the password for backup server

## Execute backup scripts
./beta_backup.sh

# Verification
## Verify backup archive on App Server 3
ls -l 

## Verify backup archive on Nautilus Backup Server
ssh clint@stbkp01
ls -l 

