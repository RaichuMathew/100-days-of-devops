# Commands Executed

## Connect to storage server 
ssh natasha@ststor01

sudo du

## Navigate to the repository
cd /usr/src/kodekloudrepos/demo

## Add the new remote named 'dev_demo'
git remote add dev_demo /opt/xfusioncorp_demo.git


## Copy the file into the current directory (the repo root)
cp /tmp/index.html .

## Stage the file for commitment
git add index.html

## Commit the change with a descriptive message
git commit -m "Added index.html from /tmp"

# Push the master branch to the dev_demo remote
git push dev_demo master

# Verification

git remote -v

