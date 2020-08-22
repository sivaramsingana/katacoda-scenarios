Let's now deploy service files for our Two-Tier Application (MongoDB/NodeJS)

`
kubectl create -f https://raw.githubusercontent.com/krishvoor/cloud_interop/master/mong-service.yaml
kubectl create -f https://raw.githubusercontent.com/krishvoor/cloud_interop/master/node-service.yaml
`{{execute}}

Let's now apply deployment files for our Two-Tier Application (MongoDB/NodeJS)

`
kubectl create -f https://raw.githubusercontent.com/krishvoor/cloud_interop/master/mong-deployment.yaml
kubectl create -f https://raw.githubusercontent.com/krishvoor/cloud_interop/master/node-deployment.yaml
`{{execute}}
