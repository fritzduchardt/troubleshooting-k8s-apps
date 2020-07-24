# Pod Head-Scratcher

## Description

The user wants to execute a couple of curls from inside his Cluster to one of his Pods. For this purpose, he wants to interactively start a `curlimages/curl` Pod. However, for some reason his "curl" Pod does not respond.

This is the command he executes: 

```
kubectl run curl-pod -it --rm --image=curlimages/curl --command bash
```

## Expected result

The curl Pod should open a shell and allow him to execute "curl" commands.