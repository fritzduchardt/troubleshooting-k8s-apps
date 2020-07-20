# StatefulSet without state

## Installation
```
kubectl apply -f problems/statefulsets/statefulset-without-state/
```

## Description

This user got stuck on a StatefulSet configuration. He uses the StatefulSet to create two web servers. Both web servers have a shared persistent volume for their static web content, e.g. HTML files.

There is a prepared HTML file called `index.html` that can be copied to the shared HD like this:

```
kubectl cp problem4/index.html web-0:/usr/share/nginx/html/
```

## Expected result

Once configured correctly, the Pods of the StatefulSet can be queried individually from the provided client Pod like this:
```
kubectl exec client -- curl web-0.nginx
kubectl exec client -- curl web-1.nginx
```
The calls should return "Hello World" 