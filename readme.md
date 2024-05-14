# ArgoCD Demo

```shell
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl apply -f namespace.yaml
kubectl apply -f application.yaml

$ kubectl get application -n argocd
NAME               SYNC STATUS   HEALTH STATUS
nginx-argocd       Synced        Healthy
namespace-argocd   Synced        Healthy

```