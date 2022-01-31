# How to

## Deploy resources

```bash
kubectl -n <namespace> apply -f <file>
```

## See resources

```bash
kubectl -n <namespace> get <resource>
```

## Delete resources

```bash
kubectl -n <namespace> delete <resource>
```

# Example: Pod

```bash
kubectl -n gofrendiasgard apply -f mypod.yaml
kubectl -n gofrendiasgard get pods
```

Accessing pod without using service

```bash
kubectl port-forward pod/nginx 3000:80
```

# Example: Replicaset

```bash
kubectl -n gofrendiasgard apply -f myreplicaset.yaml
kubectl -n gofrendiasgard get replicasets
kubectl -n gofrendiasgard get pods
```

# Example: Deployment

```bash
kubectl -n gofrendiasgard apply -f mydeployment.yaml
kubectl -n gofrendiasgard get deployments
kubectl -n gofrendiasgard get replicasets
kubectl -n gofrendiasgard get pods
```

# Example: Service

```bash
kubectl -n gofrendiasgard apply -f myservice.yaml
```

```bash
kubectl port-forward service/my-service 3000:80
```
