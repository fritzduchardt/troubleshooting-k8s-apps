# Node Port Problems

## Installation
```
 kubectl apply -f problems/ingress/node-port-problems/ 
```

## Description

A user is trying to get his application running. He wants to make it externally available via a Node Port.

Unfortunately, nothing seems to work.

You can retrieve the external IP of your Nodes with the following command:

```
kubectl get nodes -o wide
```

## Expected result

A curl to ..

```
curl [external-ip]:[external-port]/hostname
```
.. should return the hostname.