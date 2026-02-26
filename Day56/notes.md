## Task:-
Create a Kubernetes Deployment named nginx-deployment using the nginx:latest image. Ensure the container inside the deployment is named nginx-container and configure the deployment to run with 3 replicas for high availability and scalability. 

Create a NodePort type Service named nginx-service to expose the deployment. Configure the service to use nodePort 30011.

## Purpose:-
This task ensures deployment of a highly available and scalable static website using Kubernetes. The Deployment with 3 replicas provides redundancy and load distribution. The NodePort service exposes the application externally on port 30011, enabling external access to the Nginx web server running inside the cluster.
