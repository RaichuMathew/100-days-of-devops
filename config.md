# Commands Executed

## Connect to storage server

ssh natasha@ststor01 

sudo su

## Navigate to the Repository

cd /usr/src/kodekloudrepos/cluster

## Check the recent commits
git log --oneline

## Execute the Revert
git revert HEAD 

## Updating commit message 
Add 'revert cluster' 

OR

git commit --amend -m "revert cluster"

# Verification
git log --oneline
