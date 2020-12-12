# kubernetes-filebeat-metricsbeats

# Pre-Requisites:
    - Elastic Search Setup
    - Kibana Setup
    - EKS Cluster
# Elastic Search and Kibana Setup
  [Elastic Search and Kibana Setup](https://github.com/Naresh240/elasticsearch-logstash-kibana.git)
# EKS Cluster Setup:
  [EKS Cluster Setup](https://github.com/Naresh240/eks-cluster-setup/blob/main/README.md)
# Provide Elastic Search and IP in both Filebeat and Metricbeat yaml files
# Deploy filebeat and metricbeat inside our cluster
    kubectl apply -f filebeat-kubernetes.yaml
    kubectl apply -f metricbeat-kubernetes.yaml
# Check Pods using below command
    kubectl get pods -n kube-system
# Check logs in Kibana
