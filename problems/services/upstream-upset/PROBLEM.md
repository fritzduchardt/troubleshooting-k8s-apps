# Upstream Upset

## Installation
```
kubectl apply -f problems/services/upstream-upset/
```

## Description

The user has set up an upstream application that forwards calls to a downstream application, when calling the "forward" endpoint.

For some reason, something is not working regarding that call forwarding.

## Expected result

This command ..
```
kubectl port-forward service/upstream-deployment 8080
curl localhost:8080/forward/hostname
```
.. should return the hostname.