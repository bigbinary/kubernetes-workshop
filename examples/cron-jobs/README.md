####  Cron job

Create a cronjob using following command:

`$ kubectl create -f cron-job.yml`

Look at the job:

`$ kubectl get jobs`

Watch the pod status:

`$ kubectl get -w pods`

Delete a job:

`$ kubectl delete -f cron-job.yml`
