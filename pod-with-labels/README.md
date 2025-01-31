# Pod with labels

## Apply pods

```bash
kubectl apply -f hello-kube.yaml
```

## Get labels of a pod

```bash
kubectl describe pod hello-kube-api | grep -i labels
```

## Choose pod based on label

```bash
# Alternative: kubectl get pod --selector
kubectl get pod -l app=mobile
```

## Delete pods

```bash
kubectl delete -f hello-kube.yaml
```
