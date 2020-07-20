# Multiport Mixup

## Installation
```
kubectl apply -f problems/services/multiport-mixup/
```

## Description

This user is setting up a multi-container Pod where an Nginx webserver is used as a Reverse-Proxy for a Java Application.

However, the configuration seems to be not quite right.

## Expected result

The following command ..
```
kubectl port-forward service/proxied-server 8080:80
curl localhost:8080/hostname
```
-- should return the hostname.