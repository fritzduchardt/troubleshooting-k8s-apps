# Defect in Daemonset

## Installation
```
kubectl apply -f problems/daemonsets/defect-in-daemonset/
```
## Description

A user wants to install a Daemonset in order to do log aggregation on his cluster. For some reason the Pods created for his daemonset are not running

## Expected result

The command..

```
kubectl get po -o wide
```
..should show a running Daemonset Pod on each Cluster Node.