# Customized Jenkins X Pipeline for Petclinic demo

This repo is just a Petclinic demo example to be built and deploy using a non build pack Jenkins X pipeline. The original Petclinic repo is [here](https://github.com/dcanadillas/petclinic-kaniko). And the `jenkins-x.yaml` is simulating the following stages:

- Maven build of the project
- Container build and push with Kaniko
- Deploy in `jx-staging` namespace from pushed container

## Requirements

To use this repo to build the application you need to install Jenkins X:

- Install Jenkins X CLI
- Create K8s cluster and install Jenkins X platform

Then import this repo by:
```
jx import --url https://github.com/jx-dcanadillas/petclinic-jenkins-x
```
