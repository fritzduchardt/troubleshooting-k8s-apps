# Problem 2

## Installation
```
kubectl apply -f problem2
```

## Description

This customer wants to deploy his web application *socialmediaserver*. He is trying to create external availability with the Ingress Controller.

Unfortunately, he is stuck getting his application externally available.

Remember that you can retrieve your external IP can be seen on the LoadBalancer service in the kube-system namespace and can be retrieved with this command:

```
kubectl get svc --show-labels -n kube-system -l component=controller
```

## Expected result

```
kubectl port-forward service/socialmediaserver 8080
curl [external-ip]/hostname
```
Should return the hostname.