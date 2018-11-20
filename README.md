# About

This repo contain Jenkins pipeline definition for project Kentrikos.

## Requriements

Best option to use is from jenkins installed by terraform module from [kentrikos/terraform-aws-bootstrap-jenkins](https://github.com/kentrikos/terraform-aws-bootstrap-jenkins) 

Job need be run on node with installed:

* kubectl
* terraform
* jx
* helm
* tiller

## Layount

### iam

This pipeline job will generate account specific iam policies for project Kentrikos.

### kubernetes

This pipeline job will install kubernetes cluster using terraform.

### jx

This pipeline job will install Jenkins using jx installer on kubernetes.