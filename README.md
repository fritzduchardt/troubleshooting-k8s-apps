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

## Author

* Fritz Duchardt
