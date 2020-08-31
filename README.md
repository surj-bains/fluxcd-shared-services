# fluxcd-shared-services

This repo contains a set of helm and kubernetes resources to be deployed into our shared services cluster 
installed and configured by [eksctl](https://eksctl.io) through GitOps using the configuration file cluster.yaml and this respository.

```
eksctl create cluster  -f cluster.yaml
```


# Components

## flux workloads and resources provided by FluxCD

## releases for FluxCD HelmReleases

Managed Helm releases

- aws alb ingress
- certificate manager
- external secrets
- argo-cd
- aws-alb-ingress
- harbor
- jenkins-operator
- prometheus-operator
- metrics-server
- cert-manager

## workloads for Kubernetes workloads

Kubernetes resources config maps, deployments, daemonsets, namespaces, ingress and rbac