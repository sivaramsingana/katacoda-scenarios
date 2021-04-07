Let's Begin our scenario by cloning the below git repository

`git clone https://github.com/ocp-power-demos/h2o_on_ocp`{{execute HOST1 HOST2}}

Note: Before starting, Please get a license key for accessing platform.Please [sign up:](https://www.h2o.ai/try-driverless-ai/) now.

Now replace the license key available in the platform with your license key.

`vi $PWD/h2o_on_ocp/docker/experiment/license.sig`{{execute HOST2}}

Enter into docker folder

`cd $PWD/h2o_on_ocp/docker/`{{execute HOST2}}

Now create a docker image for H2O using below command

`docker build -t h2o:ppc64le .`{{execute HOST2}}

`cd ../`{{execute HOST1}}
