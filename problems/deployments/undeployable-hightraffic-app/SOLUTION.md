# Solution

- The Deployment requests more CPU cores than the cluster has to offer. Therefore, either the cluster needs more worker nodes or the resource requests of the deployment have to be reduced. Set `cpu`to 1 in the `deployment.yaml`.