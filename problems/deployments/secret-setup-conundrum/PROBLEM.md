# Secret Setup Conundrum

## Installation
```
kubectl apply -f problems/deployments/secret-setup-conundrum/ 
```
## Description

A user has developed an application that is configured with a secret. For some reason the application does not seem to start. 

## Expected result

This should return the hostname.

```
kubectl port-forward pods/[name-of-pod] 8080
curl localhost:8080/hostname
```
