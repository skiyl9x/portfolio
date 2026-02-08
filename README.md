# portfolio

I'm Oleksandr, DevOps Engineer. This is my portfolio page. I just starting my HomeLab Project)

Command to delete all resources: 

```
flux uninstall --namespace=flux-system
```

Command to bootstrap everything from scratch

```
flux bootstrap git --url=https://github.com/skiyl9x/portfolio.git --branch=main --path=clusters/dev --token-auth --namespace=flux-system
```

Enable storage-provisioner-rancher for minikube
```
minikube addons enable storage-provisioner-rancher
```
