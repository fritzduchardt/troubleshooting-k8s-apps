# Problem 1

## Installation
```
kubectl apply -f problem1
```

## Description

The customer has a deployment called *moneyapp* with a PersistentVolume and Service.


For some reason the app does not seem to response to traffic.

## Expected result

```
kubectl port-forward service/moneyapp 8080
curl localhost:8080/hostname
```
Should return the hostname.