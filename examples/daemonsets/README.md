Create a daemonset using following command

`$ kubectl create -f daemonset.yml --record`

The --record flag will track changes made through each revision.

Monitor deployment rollout status:

`kubectl rollout status deployment/nginx`

Get the basic details about daemonsets:

`$ kubectl get daemonsets/prometheus-daemonset`

More details about the daemonset:

`kubectl describe daemonset/prometheus-daemonset`

Get pods in daemonset:

`$ kubectl get pods -lname=prometheus-exporter`

Delete a daemonset:

`$ kubectl delete -f daemonset.yml`
