We will now look how to deploy the service/deployment files.

Use below commands create a running Pod

`kubectl create -f  h2o-service.yaml`{{execute}}

`service/h2o created`

`kubectl create -f h2o-deployment.yaml`{{execute}}

`deployment.apps/h2o created`
