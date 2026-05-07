# 01-intro-k8s

## Zsh
Add to ~/.zshrc
```bash
echo "alias k='kubectl'" >> ~/.zshrc
source ~/.zshrc
```

## Kubectl comandos básicos:
```bash
alias k='kubectl'
alias kgp='kubectl get pods'
alias kgs='kubectl get services'
alias kgd='kubectl get deployments'
alias kgns='kubectl get namespaces'
alias kdp='kubectl describe pod'
alias kds='kubectl describe service'
alias kdd='kubectl describe deployment'
alias kdns='kubectl describe namespace'
alias kdel='kubectl delete'
alias kapply='kubectl apply -f'
alias kcreate='kubectl create -f'
alias kex='kubectl exec -it'
alias klogs='kubectl logs'
alias kctx='kubectl config use-context'
```

## Zsh autocomplete
```bash
echo 'source <(kubectl completion zsh)' >> ~/.zshrc
echo 'complete -F __start_kubectl k' >> ~/.zshrc
source ~/.zshrc
```