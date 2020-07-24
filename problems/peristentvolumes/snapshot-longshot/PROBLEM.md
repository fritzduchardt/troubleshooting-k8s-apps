# Problem 1

## Installation

```
kubectl apply -f problems/peristentvolumes/snapshot-longshot/deployment-and-pv.yaml
```

## Description

The user is deploying an application with a persistent volume. 

Later on, he wants to backup the persistent volume by installing the following yaml:

```
kubectl apply -f problems/peristentvolumes/snapshot-longshot/volume-snapshot.yaml
```

However, the snapshot does not get created properly.


## Expected result

The snapshot should get created properly:

```
kubectl port-forward service/data-app 8080
curl localhost:8080/hostname
```