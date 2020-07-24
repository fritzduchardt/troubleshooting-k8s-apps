# Stay Alive Pod

## Installation
```
kubectl apply -f problems/deployments/stay-alive-pod/ 
```
## Description

It was supposed to be a straight forward simple deployment with five Pods, but for an unknown reason the Pods don't keep running. About half a minute after startup, the Pods crash an get restarted. This keeps on happening.

## Expected result

The Pods should run stably without restarts. 
