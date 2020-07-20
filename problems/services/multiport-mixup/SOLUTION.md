# Solution

- The port of the Nginx is pointed to 88 in the Nginx configuration, yet the Service is configured to forward traffic to port 80. Change "targetPort" to "88" in `service.yaml`.