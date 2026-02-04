# Commands Executed
## Switch to root user
sudo su -

## Install pip3 if not present
yum install -y python3-pip

## Install Ansible 4.9.0 globally using pip3
pip3 install ansible==4.9.0

## Verify Ansible installation
ansible --version

## Confirm binary path is globally accessible
which ansible

