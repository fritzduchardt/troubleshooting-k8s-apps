# Problem 6

## Installation
```
kubectl apply -f problem6
```

## Description

This user is setting up a multi-container Pod where an Nginx reverse-proxies a Java Application.

However, the configuration seems to be not quite right.

## Expected result

```
kubectl port-forward service/web-app 8080:80
curl localhost:8080/hostname
```
Should return the hostname.