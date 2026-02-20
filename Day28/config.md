# Commands Executed

## Connect to storage server
ssh natasha@ststor01

sudo su

## Navigate to the Repository
cd /usr/src/kodekloudrepos/apps

## Check the recent commits
git log --oneline

## Checkout to master branch
git checkout master

## Execute the cherry pick
git cherry-pick cd46f8a

## Push the changes to master branch
git push origin master
