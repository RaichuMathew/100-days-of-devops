# Commands Executed

##  Connect to storage server using max user
ssh max@ststor01

sudo su

## Access the repository
cd /home/max/story-blog

## Check the branch
git branch

## Pull the latest changes
git pull origin master

## Check the status and log
git status

git log --oneline
##Check the story-index.txt file for update
vi story.index.txt

Remove the wrong updates and retain clean data

## Adding, committing and pushing the changes
git add .

git commit -m 'Resolved merge conflicts'

git push origin master
