# Sample CI pipeline for equitativa

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
$ git clone https://github.com/aleksandrmironov/equitativa-sample.git
$ cd equitativa-sample/vagrant 
$ vagrant up
```

Finally you will have jenkinsCI web interface available at http://localhost:8081

##Step 2: The pipeline

You will have **equitativa-build** job available. Just press *build* (first run will be started automatically) to run the pipeline. Finally you will have the webmail app built and
available at http://localhost:8080.

Build parameters:
* imap_url (ssl://imap.gmail.com default)
* imap_port (993 default)
