 # Day 54 :- Kubernetes Shared Volumes 
## Task:-
On the jump_host, create a Pod named volume-share-datacenter with a shared volume named volume-share of type emptyDir. Configure two containers within the Pod: volume-container-datacenter-1 and volume-container-datacenter-2, both using the image fedora:latest. For each container, configure a sleep command so they remain in running state. Mount the volume volume-share at /tmp/blog in the first container and at /tmp/cluster in the second container. After the Pod is running, exec into volume-container-datacenter-1 and create a file named blog.txt under /tmp/blog. Verify that the same file is visible under /tmp/cluster in volume-container-datacenter-2.

## Purpose:-
This task validates intra-Pod data sharing using an emptyDir volume in Kubernetes. An emptyDir volume is created when the Pod starts and is shared among all containers within that Pod. Writing a file in one container and verifying it in the other confirms correct volume mounting and shared storage behavior. Running sleep ensures both containers remain active for testing and interaction.
