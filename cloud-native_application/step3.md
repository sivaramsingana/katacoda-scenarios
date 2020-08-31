Let's now deploy a cloud native application.
This repository would provide service/deployment-configuration files that can be consumed "as-is" on any OpenShift Container Platform 
as well as Kubernetes Platform - to do so, please follow below steps -

Cloning the repository -

`git clone https://github.com/krishvoor/cloud_interop` {{execute}}

Change Directories

`cd cloud_interop` {{execute}}

Let's create new Project Space -

Let's now apply service files for our Two-Tier Application -

` oc create -f mong-service.yaml ; oc create -f node-service.yaml ` {{execute}}

Let's now apply deployment files for our Two-Tier Application -

` oc create -f mong-deployment.yaml ; oc create -f node-deployment.yaml ` {{execute}}

To check status of pods -

` oc get po ` {{execute}}

Assuming pods have successfully started, let us now expose the application services outside cluster via

` oc create route edge --service=node ` {{execute}}

We can now access the Application via https://node-harsha.apps.bpradipt-2209.158.175.161.84.nip.io/api/getInspectionsByZipCodeIteration/10100/10150/1 
