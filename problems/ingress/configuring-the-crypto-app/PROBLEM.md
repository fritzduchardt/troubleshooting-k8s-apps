# Configuring the Crypto Application

## Installation
```
kubectl apply -f problems/ingress/configuring-the-crypto-app/
```
## Description

The user wants to deploy his web application *cryptoapp*. He is trying to create external availability with an Ingress Controller.

Unfortunately, things are not working and he does not know what to do.

## Expected result

```
curl [external-ip]/cryptoapp/hostname
```
Should return the hostname.