# Sample CI pipeline for fetchr

#Tool stack

* Vagrant
* Docker
* Jenkins
* Ansible

Here is a short HowTO:

## Step 1: Prepare a CI environment

Requirements: vagrant (tested w/ vagrant==2.0.1 and virtualbox==5.1.30 at MacOS 10.13.2)

Shell steps:

```bash
$ git clone https://github.com/aleksandrmironov/fetchr-samples.git
$ cd fetchr-samples/vagrant 
$ vagrant up
```

Finally you will have jenkinsCI web interface available at http://localhost:8081

##Step 2: The pipeline

You will have **fetchr-build** job available. Just press *build* or make changes
in hello-world.git to run the pipeline. Finally you will have the app built and
available at http://localhost:8080.

