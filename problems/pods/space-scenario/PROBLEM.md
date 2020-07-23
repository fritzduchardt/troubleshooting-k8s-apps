# Problem 11

## Installation

kubectl apply -f problems/pods/space-scenario/ 

## Description

The user has a Pod running that writes huge amounts of data to the file system. This seems to cause to Pod to get evicted.

You can simulate this by calling the following endpoint on the Pod:

```
kubectl port-forward pods/spacefiller 8080
curl localhost:8080/space/200
```

## Expected result

The Pod has to keep running after calling the endpoint above.