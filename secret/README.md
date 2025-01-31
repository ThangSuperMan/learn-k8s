# Secrets

# Convert plan text base64 format

```bash
echo 'you text here' | base64
```

## Decode base64

```bash
kubectl get secrets database-credentials -o jsonpath="{.data.MYSQL_ROOT_USER}" | base64 --decode
```
