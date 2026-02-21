# Commands Executed
## Connect to storage server
ssh tony@stapp01

sudo su

## Copy file to docker container

docker cp /tmp/nautilus.txt.gpg 4062dd318f2c:/tmp/

# Verification
docker exec 406 ls -l /tmp/

If you run ls -l /tmp/, you are looking at the temporary folder on your host machine (your laptop or server). By prefixing it with docker exec 406, you are "teleporting" that command so it only looks at the /tmp/ folder inside that specific container's isolated environment.

# Output

-rw-r--r-- 1 root root 105 Feb 21 15:33 nautilus.txt.gpg
