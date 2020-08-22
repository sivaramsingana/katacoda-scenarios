What's best way to test a cloud-native application than Kubernetes ?

`wget https://dl.k8s.io/v1.18.0/kubernetes-client-darwin-386.tar.gz 
tar -zxf kubernetes-client-darwin-386.tar.gz
cp kubernetes/client/bin/kubectl ~/.bin/kubectl
`{{execute}}

The client uses the environment variable KUBERNETES_MASTER to define the default Master to communicate with.

`export KUBERNETES_MASTER=http://docker:8080`{{execute}}
