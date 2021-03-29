Let's Begin our scenario by cloning the below git repository

`git clone https://github.com/ocp-power-demos/h2o_on_ocp`{{execute}}

Enter into docker folder

`cd $PWD/h2o_on_ocp/docker/`{{execute}}

Now create a docker file for H2O using below command

`docker build -t h2o:ppc64le .`{{execute}}

`cd ../`{{execute}}
