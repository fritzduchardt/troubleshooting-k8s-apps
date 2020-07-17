# Problem 8

## Installation
```
kubectl apply -f problem11
```

## Description

Your customer is trying to setup two things: a Pod that can be queried directly via a headless Service and a StatefulSet with Pods that can be queried directly.

However, the configuration does not work. Please investigate.

## Expected result

From the provided Netshoot Pod the following curls should work fine:

Calling the single Pod:
```
curl [Pod-Name].[Service-Name]
```
Calling the StatefulSet Pods, e.g.
```
curl [Pod-Name].[Service-Name]
```
