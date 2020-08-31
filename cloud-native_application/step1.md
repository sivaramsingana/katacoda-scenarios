What's best way to test a Cloud Native Application than OpenShift Container Platform running on IBM Power Virtual Servers ?

Let us pull a ubuntu playground ( as we have better control to install additional packages )

` docker run -it ubuntu bash
`{{execute}}

`apt update; apt install wget git -y`{{execute}}

We will leverage `oc` commands to interact with OCP4.5, we will first download `oc` tarball 

`wget https://downloads-openshift-console.apps.bpradipt-505b.161.156.154.131.nip.io/amd64/linux/oc.tar`{{execute}}

Unpacking Tarball

`tar -xf oc.tar` {{execute}}

Updating path variable

`export PATH=$PATH:$PWD`{{execute}}
