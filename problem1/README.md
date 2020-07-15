# Problem 1

## Installation
```
kubectl apply -f problem1
```

## Description

The user is stuck on installing a Daemonset to the cluster for log aggregation.

## Expected result

```
kubectl get po -o wide
```
A pod should be running on every cluster node