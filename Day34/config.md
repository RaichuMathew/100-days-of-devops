# Commands Executed

## Connect to storage server
ssh natasha@ststor01

sudo su

## Navigate to the repository

cd /opt/news.git/hooks

ls


## Add the below in post-update file
vi post-update

#!/bin/bash

for refname in "$@"; do
  if [ "$refname" = "refs/heads/master" ]; then
    today=$(date +%F) 
    tag_name="release-${today}" # relase-2023-06-15

    newrev=$(git rev-parse "$refname")

    git tag -f "$tag_name" "$newrev"
  fi
done

## Give executable permission 
chmod +x post-update

## Navigate to cloned repo 
cd /usr/src/kodekloudrepos

## Check git branches and changes
git branch

git log --oneline

## Feauture branch has changes that are not pushed to master branch
git checkout master

git log --oneline

## Merge changes of feature to master
git merge feature

git push origin master


