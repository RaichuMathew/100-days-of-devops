# Commands Executed
## Connect to storage server
ssh natasha@ststor01
sudo su
## Navigate to the repository
/usr/src/kodekloudrepos/demo

## Verify the History
git log --oneline
## Perform the Hard Reset
git reset --hard 0b0485f
## Synchronize the Remote
git push origin main
# Verification
git log --oneline
