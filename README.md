# aidtech

For the purpose of the test we have deployed a rancher server with terraform. 
Stack we used:
* terraform
* rancher
* jenkins

## Rancher
* used to provision k8s clusters
* manage helm charts
* define node templates

## Jenkins
* ci/cd pipeline
* integration with github
* integration with kubernetes via service account
* trigger redeployment of hello-world chart (demo nodejs application)

## ChartMuseum
* deployed but not used

## Deployment flow:
* create a pull request from your branch onto the `master` branch

Case 1: tests pass
* deployment is triggered

Case 2: tests fail
* deployment is halted


https://18.216.195.0
admin / [obscured]
