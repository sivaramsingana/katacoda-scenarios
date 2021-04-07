To check the status of pods in your desired namespace issue the following

`kubectl get po -n default`{{execute}}

`NAME                    READY      STATUS     RESTARTS    AGE`

`h2o-5fcc88f885-8jdck    1/1        Running    0           1m`

Note: Please save name of the pod for future use.

Let's test our work!!

Now shell into h2o container.

`kubectl exec --stdin --tty <Name of the pod> -- /bin/bash`{{copy}}
