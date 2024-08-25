# Multi-Cluster-Monitoring
Multi cluster monitoring using Grafana, Victoria Metrics in GCP
```
Infra
- Cloud: GCP
- Global VPC: GCP
- GKE: 1.28
- Nginx Ingress
- Victoria Metrics Cluster HA
- Grafana HA with Database as backend
- Kustomization + Helm
- Blackbox Exporter to check API health
```



```mermaid

graph TD
C[(vm-agent-cluster1)] --> B
D[(vm-agent-cluster2)] --> B
E[(vm-agent-cluster3)] --> B
B((Victoria Metrics Cluster 
Master )) --> Metrics --> A(( Grafana ))

```