Create a deployment using following command

`$ kubectl create -f deployment.yml --record`

The --record flag will track changes made through each revision.

Create a service for deployment using following command

`$ kubectl create -f service.yml`

Monitor deployment rollout status:

`kubectl rollout status deployment/nginx`

Get the deployments:

`$ kubectl get deployments`

Describe the deployment for details:

`$ kubectl describe deployment nginx`

A Deployment creates a ReplicaSet to manage the number of replicas

`$ kubectl get replicaset`

Scaling a deployment:

`$ kubectl scale --replicas=5 deployment/nginx`

Update a deployment:

`$ kubectl edit deployment/nginx`

`$ kubectl set image deployment/nginx nginx=nginx:1.9.1`

Rollout status of a deployment:

`$ kubectl rollout history deployment/nginx`

Rollback a deployment:

`$ kubectl rollout undo deployment/nginx`

Delete a deployment:

`$ kubectl delete deployment/nginx`
