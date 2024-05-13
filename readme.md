# ArgoCD Demo

```shell
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl apply -f namespace.yaml
kubectl apply -f application.yaml

$ kubectl get application -A
NAMESPACE   NAME           SYNC STATUS   HEALTH STATUS
argocd      nginx-argocd   Synced        Healthy


```