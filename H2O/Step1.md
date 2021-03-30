Let's Begin our scenario by cloning the below git repository

`git clone https://github.com/ocp-power-demos/h2o_on_ocp`{{execute HOST1}}

Enter into docker folder

`cd $PWD/h2o_on_ocp/docker/`{{execute HOST1}}

Now create a docker file for H2O using below command

`docker build -t h2o:ppc64le .`{{execute HOST1}}

`cd ../`{{execute HOST1}}
