# Solution

- In `service.yaml` correct the label selector of the deployment: change `app: apigateway` to `app: api-gateway`.
- In `service.yaml` correct the target port. It should be 80 rather than 8080.