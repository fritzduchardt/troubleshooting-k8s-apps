# Problem 7

## Installation
```
kubectl apply -f problem6
```

## Description

Here we are having two Deployment - upstream and downstream. The upstream application calls downstream when calling the "forward" endpoint.

But something is not working regarding that call forwarding.

## Expected result

```
kubectl port-forward service/upstream-deployment 8080
curl localhost:8080/forward/hostname
```
Should return the hostname.