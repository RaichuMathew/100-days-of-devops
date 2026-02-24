# Day50 :- Set Resource Limits in Kubernetes Pods 

## Task:-
On the jump_host, create a Pod named httpd-pod with a container named httpd-container using the image httpd:latest. Configure the container to have resource requests of 15Mi memory and 100m CPU, and resource limits of 20Mi memory and 100m CPU. Apply the configuration using kubectl and verify that the Pod is running with the specified resource constraints.

## Purpose:-
This task enforces resource management within the Kubernetes cluster by defining CPU and memory requests and limits. Requests ensure the scheduler allocates sufficient resources for the Pod, while limits prevent the container from consuming excessive resources. Proper configuration helps maintain cluster stability, prevent resource starvation, and improve overall application performance management.
