# Manage resources with namespace

## Get all namespaces

```bash
## Alternative: kubectl get namespaces
kubectl get ns
```

> NOTES: by default the K8s will create for us the default namespace named: `default`

## Create new namespace

```bash
kubectl create ns testing
```

> NOTES: standard when create a namespace with the following format: `<project_name>-<environment>`. Examples: hi-testing, hi-staging, hi-production

## Create namespace and pods

```bash
kubectl apply -f manage-resources-with-namespace/hello-namespace.yaml
```

## Get pods based on namespace

```bash
kubectl get pods -n testing
```

## Delete namespace and pod

```bash
kubectl delete -f manage-resources-with-namespace/hello-namespace.yaml
```
