# fluxcd-shared-services

This repo contains a set of helm and kubernetes resources to be deployed into our shared services cluster 
installed and configured by [eksctl](https://eksctl.io) through GitOps.



## Components

- [Cluster autoscaler](https://github.com/kubernetes/autoscaler/tree/master/cluster-autoscaler) -- to [automatically add/remove nodes](https://aws.amazon.com/premiumsupport/knowledge-center/eks-cluster-autoscaler-setup/) to/from your cluster based on its usage.
- [Prometheus](https://prometheus.io/) (its [Alertmanager](https://prometheus.io/docs/alerting/alertmanager/), its [operator](https://github.com/coreos/prometheus-operator), its [`node-exporter`](https://github.com/prometheus/node_exporter), [`kube-state-metrics`](https://github.com/kubernetes/kube-state-metrics), and [`metrics-server`](https://github.com/kubernetes-incubator/metrics-server)) -- for powerful metrics & alerts.
- [Grafana](https://grafana.com) -- for a rich way to visualize metrics via dashboards you can create, explore, and share.
- [Fluentd](https://www.fluentd.org/) & Amazon's [CloudWatch agent](https://aws.amazon.com/cloudwatch/) -- for cluster & containers' [log collection, aggregation & analytics in CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Container-Insights-setup-logs.html).
