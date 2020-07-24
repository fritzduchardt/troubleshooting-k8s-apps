# Pairing Pods (Only for multi-node cluster)

```
kubectl apply -f problems/pods/pairing-pods/ 
```

## Description

The user wants to deploy several Pods that write to the same shared volume.

He starts his Pods and then uses `exec` to log into them. There, he looks at the folder `/shared` to see whether this is shared between Pods. 

Unfortunately, this does not work for him.

This is the command he executes to log into the Pods: 

```
kubectl exec -it [name-of-the-pod] -- bash
```

**Hint:** this is how you can view your node labels:
```
kubectl get nodes --show-labels
```

## Expected result

Folder `shared` should be shared between Pods. Files written to this folder from one Pod should be visible to the other Pod.