# Commands Executed

## Generate the Manifest
k run pod --image nginx:latest --dry-run=client -o > pod.yaml

## Insert the following in pod.yaml file

vi pod.yaml

apiVersion: v1
kind: Pod
metadata:
  labels:
    app: nginx_app
  name: pod-nginx
spec:
  containers:
  - image: nginx:latest
    name: nginx-pod

## Apply the Change
k apply -f pod.yaml

# Verification 
k get po
