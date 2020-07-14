# Problem 5

## Installation
```
kubectl apply -f problem5
```

## Description

A user is trying to get his deployment running and wants to make it externally available with a Node Port service.

Unfortunately, nothing seems to work.

## Expected result

```
curl [external-ip]:[external-port]/hostname
```
Should return the hostname.