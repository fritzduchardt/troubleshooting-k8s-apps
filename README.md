# Troubleshooting K8s Applications

## Usage

Create a dedicated namespace, e.g.:
```
kubectl create namepace trouble
```
Make this your default namespace, e.g.:
```
kubectl config set-context --current --namespace=trouble
```
Install a problem, e.g. 
```
kubectl create -f problems/deployments/problem-with-money/
```
Read the `PROBLEM.md` for an introduction to the problem. Fix the problem - if need be consult the `SOLUTION.md`.

Once ready to move on to the next problem, delete the resources in your namespace:
```
kubectl delete all --all
```

## Order of difficulty

### Easy Problems

- deployments/stay-alive-pod
- deployments/configmaps-are-tricky
- deployments/undeployable-hightraffic-app
- deployments/defect-deployment
- daemonsets/defect-in-daemonset
- jobs/job-incomplete
- services/out-of-service

### Medium Problems
- deployments/secret-setup-conundrum
- ingress/node-port-problems
- pods/pod-head-scratcher
- pods/space-scenario
- services/upstream-upset
- peristentvolumes/snapshot-longshot

### Hard Problems
- ingress/configuring-the-crypto-app
- ingress/social-media-disconnected
- jobs/mangled-migration
- persistentvolumes/dataapp-and-its-volume
- persistentvolumes/webapp-wont-work
- services/headless-pod
- services/multiport-mixup
- statefulsets/statefulset-without-state




## Author

* Fritz Duchardt
