# Solution

- The Pods are not necessarily deployed to the same worker node. This can be enforced with a `nodeSelector`, e.g. by adding this to the deployment.yaml:
```
      nodeSelector:
        kubernetes.io/hostname: [name-of-one-of-your-nodes]
```
