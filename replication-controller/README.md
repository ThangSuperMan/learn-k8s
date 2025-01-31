# Replication Controllers (RC)

## Main components in RC

- Desired replica count
- Pod template
- Selectors: RC use selector to target and manage pods
- Self-healing: Auto remove the error pod

## Apply pods

```bash
kubectl apply -f hello-kube.yaml
```

## Replication controllers flow

#### Flow when apply the new update

![image](./images/replication-controller-flow.avif)

#### Auto create the pods when the current running node down/crashed

![image](./images/auto-create-pods-in-another-node.avif)

## Create new node in the minikube cluster

```bash
minikube start --nodes 2 -p node
```

## List all nodes

```bash
kubectl get nodes
```

## Label the node

```bash
kubectl label node node-m02 node-role.kubernetes.io/worker=worker
```
