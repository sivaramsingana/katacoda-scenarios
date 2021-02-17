Let's now deploy the sameple application.

Cloning the repository

`git clone https://github.com/ocp-power-demos/cloud_interop`{{execute}}

This repository contains the service and deployment configuration files that can be used as-is on the OpenShift or any Kubernetes platform.

Change Directory

`cd cloud_interop`{{execute}}

Create a new `Project`

`oc new-project sample`{{execute}}

Deploy the application

`oc create -f mong-service.yaml; oc create -f node-service.yaml;  oc create -f mong-deployment.yaml;  oc create -f node-deployment.yaml `{{execute}}

Check status of Pods

`oc get pods `{{execute}}

Assuming pods have successfully started, let us now expose the application services outside cluster via

`oc create route edge --service=node `{{execute}}

You can now access the application via https://node-sample.apps.test-ocp-ce4a.161.156.153.93.xip.io/api/getInspectionsByZipCodeIteration/10100/10150/1
