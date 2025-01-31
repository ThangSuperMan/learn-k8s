# Pod

## Build docker image

```bash
docker build . -t hello-kube:latest
```

## Check container

```bash
docker run -d --name hello-kube -p 3000:3000 hello-kube:latest
```

## Check connection

```bash
curl localhost:3000
```

## Apply pod

```bash
kubectl apply -f hello-kube.yaml
```

## Port forwarding from host to pod

```bash
kubectl port-forward pod/hello-k8s 3002:3000
```

## Delete a pod

```bash
kubectl delete pod hello-kube
```
