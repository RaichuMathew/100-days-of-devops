# Commands Executed

## Connect to storage server
ssh natasha@ststor01 

sudo su

## Navigate to the repository
cd /usr/src/kodekloudrepos/games

## Check recent commits of feature branch
git log --oneline
## Check reecent commits of master branch
git checkout master

git log --oneline

git pull origin master
## Rebasing to have the feature branch updated
git checkout feature

git rebase master

## Force pushing changes 
git push origin feature -f
