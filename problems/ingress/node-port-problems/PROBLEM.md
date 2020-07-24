# Node Port Problems

## Installation
```
 kubectl apply -f problems/ingress/node-port-problems/ 
```

## Description

A user is trying to get his application running. He wants to make it externally available via a Node Port.

Unfortunately, nothing seems to work.

## Expected result

Retrieve an external IP from one of your nodes with:

```
kubectl get nodes -o wide
```

Retrieve the external port (the one in range o 30000-32767) of the "web-app" service with:
```
kubectl get service
```

A curl to ..

```
curl [external-ip]:[external-port]/hostname
```

.. should return the hostname.