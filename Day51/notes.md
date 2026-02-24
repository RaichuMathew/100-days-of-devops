# Day51 :- Rolling Update in Kubernetes
## Task:-
On the jump_host, perform a rolling update on the existing deployment named nginx-deployment to use the image nginx:1.17. Apply the update using kubectl, ensuring the image tag is explicitly specified. Monitor the rollout status to confirm the update progresses successfully and verify that all updated Pods are in a running and ready state after completion.

## Purpose:-
This task validates controlled application updates in Kubernetes using a rolling update strategy. Updating the image to nginx:1.17 ensures the deployment runs the new application version. A rolling update replaces Pods incrementally, maintaining service availability and minimizing downtime. Verifying rollout status ensures cluster stability and confirms successful deployment of the updated application version.
