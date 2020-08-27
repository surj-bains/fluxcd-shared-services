# fluxcd-shared-services

This repo contains a set of helm and kubernetes resources to be deployed into our shared services cluster 
installed and configured by [eksctl](https://eksctl.io) through GitOps the configuration file cluster.yaml.

```
eksctl create cluster  -f cluster.yaml
```



See https://github.com/polarpoint-io/fluxcd-quick-start-shared-services-base for the quickstart base kubernetes workloads for monitoring, cluster autoscaling, fluentd. and pulled into the base


## Components

- flux workloads and resources provided by FluxCD
- base default and base resources
- releases for FluxCD HelmReleases
- workloads for Kubernetes workloads

