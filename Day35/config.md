# Commands Executed
## Connect to storage server
ssh banner@stapp02

sudo su

## Check centos version
vi /etc/*release*/

## Remove Conflicts and Add Repository
sudo dnf remove -y podman buildah

sudo dnf install -y yum-utils

sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

## Install Docker Engine and Compose:

sudo dnf install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin


## Start and Enable Docker:
sudo systemctl enable --now docker

