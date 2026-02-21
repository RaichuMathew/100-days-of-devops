# Commands Executed

## Connect to App server 3
ssh banner@stapp03

sudo su
## Pull image
docker pull busybox:musl
## Re-tagging the image
docker tag busybox:musl busybox:news
