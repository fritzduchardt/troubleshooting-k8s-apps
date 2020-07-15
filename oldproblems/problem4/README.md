# Problem 4

## Installation
```
kubectl apply -f problem4
```

## Description

Your customer has developed an application that is configured with a config map. For some reason the app does not seem to start. 

## Expected result

```
kubectl port-forward pods/[name-of-pod] 8080
curl localhost:8080/hostname
```
Should return the hostname.