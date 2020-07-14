# Problem 3

## Installation
```
kubectl apply -f problem3
```

## Description

For his application "web-app", your customer can't get his Pods running.

For some reason the app does not seem to response to traffic.

## Expected result

```
kubectl port-forward service/web-app 8080
curl localhost:8080/hostname
```
Should return the hostname.