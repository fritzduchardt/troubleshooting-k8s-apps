# Solution

- The Ingress pass is not set correctly. In `ingress.yaml` change "/sms" to "/sms/(.*) 
- The Service selector is not pointing to the Deployment. In `service.yaml` change: 
```
  selector:
    app: social-media-server
```
to:
```
  selector:
    app: socialmediaserver
```
