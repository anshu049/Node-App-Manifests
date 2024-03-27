# Installation
(https://argo-cd.readthedocs.io/en/stable/getting_started/)

`kubectl create namespace argocd`

`kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`

`modify service/argocd-server for Argo UI`

## Initial paasword
`kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d && echo`
