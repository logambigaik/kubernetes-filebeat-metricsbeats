# kubernetes-filebeat-metricsbeats

# Pre-Requisites:
    - Install Elastic Search
    - Install Kibana
    - EKS Cluster
# Provide Elastic Search and IP in both Filebeat and Metricbeat yaml files
# Deploy filebeat and metricbeat inside our cluster
    kubectl apply -f filebeat-kubernetes.yaml
    kubectl apply -f metricbeat-kubernetes.yaml
# Check Pods using below command
    kubectl get pods -n kube-system
# Check logs in Kibana
