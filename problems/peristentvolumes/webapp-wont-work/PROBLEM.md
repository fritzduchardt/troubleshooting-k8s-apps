# Webapp won't work

## Installation
```
kubectl apply -f problems/peristentvolumes/webapp-wont-work/  
```

## Description

The user can't get his web application working and hooked up to a persistent volume.

For some reason the application does not seem to response to traffic.

## Expected result

```
kubectl port-forward service/web-app 8080
curl localhost:8080/hostname
```
Should return the hostname.