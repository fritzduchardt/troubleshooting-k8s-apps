# Headless Pod

## Installation
```
kubectl apply -f problems/services/headless-pod/
```

## Description

The user is trying to set up a Pod that can be queried directly via a headless Service.

However, he is not able to call the Pod via a DNS name.

## Expected result

From the provided Netshoot Pod the following curl command should work fine:
```
curl [Pod-Name].[Service-Name]
```
```
