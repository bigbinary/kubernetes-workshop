#### Namespaces

Create a namespace:

`$ kubectl create -f namespace.yml`

Look at the namespace:

`$ kubectl get namespaces`

Get the resources in namespaces

`$ kubectl -n get all`

Delete a job:

`$ kubectl delete -f namespace.yml`

#### Resource Quota and Limits


Create limits:
```
kubectl apply -f resource-quota.yaml
resourcequota "quota" created
```

This limit specifies

* Every new Container created must have a memory and CPU limit

* Total number of Pods in this namespace cannot exceed 10

* Total number of ReplicationController in this namespace cannot exceed 3

* Total number of Service in this namespace cannot exceed 5

* Total number of ConfigMap in this namespace cannot exceed 5