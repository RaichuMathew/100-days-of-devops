# Day48 :- Deploy Kubernetes Pod in cluster

## Task:-
On the jump_host, use kubectl to create a Pod named pod-nginx using the image nginx:latest. Configure the Pod with a label app=nginx_app and ensure the container inside the Pod is named nginx-container. Verify that the Pod is successfully created and running in the cluster.

## Purpose:-
This task validates basic Kubernetes workload deployment using kubectl. Creating a Pod with a specific image tag ensures controlled image version usage. Applying the required label supports identification and future service or selector-based operations. Naming the container explicitly enforces correct specification structure and confirms proper Pod configuration within the Kubernetes cluster.
