# Problem 1

## Installation
```
kubectl apply -f problems/peristentvolumes/dataapp-and-its-volume/
```
## Description

The user is trying to deploy an application called *data-app* that writes an excessive amount of data.

For some reason the application does not seem to response to traffic.

## Expected result

```
kubectl port-forward service/data-app 8080
curl localhost:8080/hostname
```
Should return the hostname.