# Undeployable High-Traffic App

## Installation
```
kubectl apply -f problems/deployments/undeployable-hightraffic-app/
```

## Description

The user wants to deploy an application to handle a lot of traffic. Therefore, the application has a lot of replicas. However, he can't get some of the Pods to run.

## Expected result

All Pods of the Deployment should be running.