# cubix-cloudnative-block4-homework

Miskovits Dániel

# Kustomize installation / deployment commands for PROD

```
kubectl apply -k overlays/prod
kubectl delete -k overlays/prod
```

# Kustomize installation / deployment commands for TEST

```
kubectl apply -k overlays/test
kubectl delete -k overlays/test
```

# Kustomize installation / deployment commands for DEV

```
kubectl apply -k overlays/dev
kubectl delete -k overlays/dev
```

# Helm installation / deployment commands for PROD

```
kubectl create namespace hw4-prod
helm install prod hw4 -n hw4-prod -f .\values-prod.yaml
helm uninstall prod -n hw4-prod
kubectl delete namespace hw4-prod
```

# Helm installation / deployment commands for TEST

```
kubectl create namespace hw4-test
helm install test hw4 -n hw4-test -f .\values-test.yaml
helm uninstall test -n hw4-test
kubectl delete namespace hw4-test
```

# Helm installation / deployment commands for DEV

```
kubectl create namespace hw4-dev
helm install dev hw4 -n hw4-dev -f .\values-dev.yaml
helm uninstall dev -n hw4-dev
kubectl delete namespace hw4-dev
```
