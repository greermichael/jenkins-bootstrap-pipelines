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

##### auto 

This job handle s3 state and create policies on account

##### manual

This job do not use remote state and only generate policy files 

### kubernetes

This pipeline job will install kubernetes cluster using terraform.

### jx

This pipeline job will install Jenkins using jx installer on kubernetes.