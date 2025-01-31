# ReplicaSets (RS)

## Replication features

- Manage pods by labels like RC
- Allow to multiple select the labels
- Allow to use matchExpression for selector

## Operation in mat matchExpression

- In, NotIn, Exists, DoesNotExist

## DaemonSets

- Allow us to tell with K8s that we want to add a pod per node in cluster

> NOTES: we usally use this feature for logging from node by doing this
> we can prevent the case duplicate logs because two or more than two pods can run in the same node

## Label of node

```bash
# Command for getting node names: kubectl get nodes
kubectl label nodes node disk=ssd
```

## Overwrite existing label of node

```bash
kubectl label nodes node disk=ssd --overwrite
```
