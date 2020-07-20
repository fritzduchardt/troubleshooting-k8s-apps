# Configuration is tricky

## Installation
```
kubectl apply -f problems/deployments/configuration-is-tricky/ 
```
## Description

A user has developed an application that is configured with a config map. For some reason the application does not seem to start. 

## Expected result

This should return the hostname.

```
kubectl port-forward pods/[name-of-pod] 8080
curl localhost:8080/hostname
```
