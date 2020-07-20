# Social Media Disconnected

## Installation
```
 kubectl apply -f problems/ingress/social-media-disconnected/ 
```

## Description

This user wants to deploy his web application *socialmediaserver*. He is trying to create external availability via his Ingress Controller.

Unfortunately, this does not work.

You can retrieve your external IP on the LoadBalancer service in the kube-system namespace like this:

```
kubectl get svc --show-labels -n kube-system -l component=controller
```

## Expected result

The following command ..
```
curl [external-ip]/sms/hostname
```
.. should return the hostname.