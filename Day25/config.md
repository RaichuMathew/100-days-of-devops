# Commands Executed

## Login to Storage Server
ssh natasha@ststor01

sudo su
## Navigate to Cloned Repository
cd /usr/src/kodekloudrepos/blog

## Verify Current Branch
git branch

## Create New Branch datacenter from master
git checkout master

git checkout -b datacenter
## Copy index.html into Repository
cp /tmp/index.html .

## Verify File Presence
ls -l

## Commit Changes in datacenter Branch
git add .

git commit -m 'Initial commit'

## Switch Back to Master Branch
git checkout master

## Merge datacenter Branch into master
git merge datacenter

## Pushing the changes to master branch
git push origin master
