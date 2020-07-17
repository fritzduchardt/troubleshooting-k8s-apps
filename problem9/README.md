# Problem 9

## Installation

Not required 

## Description

The user wants to execute a couple of curls into one of his Pods. For that purpose he wants to start a dedicated Curl Pod in an interactive session. However, for some reason his curl Pod does not keep running.

This is the command he is executing: 

```
kubectl run curl-pod -it --rm --image=curlimages/curl --command bash
```

## Expected result

The curl Pod should keep running.