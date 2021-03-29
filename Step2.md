We will now look how to deploy the service/deployment files.

Note: Please replace `kubectl` with `oc` if you are using Redhat Openshift

`kubectl create -f  h2o-service.yaml`{{execute}}

`service/h2o created`

`kubectl create -f h2o-deployment.yaml`{{execute}}

`deployment.app/h2o created`
