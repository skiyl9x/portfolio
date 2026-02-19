## My HomeLab Project TODOs
- [x] Create Skeleton for GitHub Repository with Flux
- [x] Implement Rendered Manifests Flux approach
- [x] Add Traefik as API Gateway to allow access to the resources through domain names
- [x] Install Prometheus+Grafana stack
- [x] Upgrade FluxCD to use Flux Operator
- [x] Install RabbitMQ Cluster Operator and add RabbitMQ Cluster
- [x] Implement fist Helm Chart for Web Application
- [x] Create Helm Repository (OCI), upload Helm Templates and use them
- [x] Install two services and connect them
- [ ] Add automatic certificate generation with Traefik for applications
- [ ] Try Service Mesh, connect services to each other
- [ ] Change FluxCD architecture, use OCI artifacts instead of code in GitHub branches to deploy
- [ ] Go through all your current deployments (RabbitMQ, Prometheus, etc.) and explicitly set resources.requests and resources.limits. Try to "OOMKill" (Out of Memory Kill) a pod by setting a limit too low to see how Kubernetes reacts.
- [ ] Implement Pod Anti-Affinity
      If you have more than one node, configure your web app deployment so that two replicas never run on the same physical node.
- [ ] Implement limitation of resources for namespaces
- [ ] Add OpenTelemetry collector to collect the logs and push to Loki
- [ ] Create matrix job for frontend and backend and dynamic image name from docker-bake.hcl
