# Commands Executed
## To get List All Deployments
k get deploy
## To get list All Pods
k get po
## Update Container Image
k set image deploy nginx-deployment nginx-container=nginx:1.17
## View Deployment Revision History
k rollout history deploy nginx-deployment
