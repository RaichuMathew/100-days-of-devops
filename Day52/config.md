# Commands Executed

## To get the existing deployment
k get deploy -o wide
## Check the recent history
kubectl rollout history deploy nginx-deployment
## Refresh the kubectl every second to see the pods getting terminated during rollout
watch -n 1 kubectl po
## Reverting the changes to previous revision
kubectl rollout undo deploy nginx-deployment
