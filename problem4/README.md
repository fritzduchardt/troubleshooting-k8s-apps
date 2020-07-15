# Problem 4

## Installation
```
kubectl apply -f problem4
```

## Description

This user got stuck on a StatefulSet configuration. He uses the StatefulSet to create two webservers. Both web servers have a shared persistent volume.

There is a prepared HTML file called index.html that can be copied on the shared HD like this:

```
kubectl cp problem4/index.html web-0:/usr/share/nginx/html/
```

## Expected result

```
kubectl exec client -- curl web-0.nginx
kubectl exec client -- curl web-1.nginx
```
Should return "Hello World" 