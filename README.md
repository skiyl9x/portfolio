# portfolio

I'm Oleksandr, DevOps Engineer. This is my portfolio page. I just starting my HomeLab Project)

Command to delete all resources: 

```
flux uninstall --namespace=flux-system
```

Command to bootstrap everything from scratch

```
flux bootstrap git --url=ssh://git@github.com/skiyl9x/portfolio --branch=main --private-key-file=../github-fluxcd-portfolio --password=fluxcd --path=clusters/dev --namespace=flux-system
```

Enable storage-provisioner-rancher for minikube
```
minikube addons enable storage-provisioner-rancher
```
