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



Traefik installation
```
minikube addons enable metallb
```

```
oshyd@1H851821G3:~/MyProjects/portfolio/infrastructure/base/configs/metallb$ minikube ip
192.168.39.162
oshyd@1H851821G3:~/MyProjects/portfolio/infrastructure/base/configs/metallb$ minikube addons configure metallb
-- Enter Load Balancer Start IP: 192.168.39.180
-- Enter Load Balancer End IP: 192.168.39.200
    ▪ Using image quay.io/metallb/speaker:v0.9.6
    ▪ Using image quay.io/metallb/controller:v0.9.6
✅  metallb was successfully configured
```

Add next to the /etc/hosts
```
192.168.39.180  traefik-dashboard.minikube.cluster whoami.minikube.cluster nginx.minikube.cluster rabbitmq.minikube.cluster flux-web.minikube.cluster grafana.minikube.cluster
```


Create secret

```
kubectl create secret docker-registry github-oci-auth --namespace=flux-system --docker-server=ghcr.io --docker-username=skiyl9x --docker-password=<github-token>
```
