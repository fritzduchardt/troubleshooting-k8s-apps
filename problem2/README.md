# Problem 2

## Installation
```
kubectl apply -f problem2
```

## Description

This customer wants to deploy his web application *crypto-application*. He is trying to create external availability with the Ingress Controller.

Unfortunately, he is stuck getting his application externally available.

## Expected result

```
curl [external-ip]/hostname
```
Should return the hostname.