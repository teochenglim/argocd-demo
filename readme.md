# ArgoCD Demo

```shell
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl create ns local-argo
kubectl apply -f application.yaml
```