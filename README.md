Install argoCD:

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

Expose argoCD UI:

kubectl port-forward -n argocd svc/argocd-server 8080:443
