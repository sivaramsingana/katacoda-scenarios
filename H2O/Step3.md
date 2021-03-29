To check the status of pods in your desired namespace issue the following

`kubectl get po -n default`{{execute}}

`NAME                    READY      STATUS     RESTARTS    AGE`

`h2o-5fcc88f885-8jdck    1/1        Running    0           1m`

Note: Please save name of the pod for future use.

Let's test our work!!

If you're using openshift then execute below command

`oc rsh <Name of pod>`{{copy}}

Note: Use the name saved above.

If you're using kubernetes then execute below command.

`kubectl exec --stdin --tty <Name of the pod> -- /bin/bash`{{copy}}
