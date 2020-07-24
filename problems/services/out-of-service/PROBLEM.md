# Out of Service

## Installation
```
kubectl apply -f problems/services/out-of-service/
```

## Description

The user wants to expose a deployment via a service. However, once he opens a port-forwarding there is no response from the service. What did he do wrong?

## Expected result

The following command ..
```
k port-forward service/api-gateway 8080:80 
curl localhost:8080
```
-- should return the hostname.