 # Commands Executed
## Connect to storage server
ssh natasha@ststor01
sudo su

## Navigate to the repository
cd /usr/src/kodekloudrepos/ecommerce
## To get a list of stash available
 git stash list


## Restore the stash at 1
 git stash pop stash@{1}
## Commit and push the changes to master
 git commit -m 'Initial commit'

 git push origin master
