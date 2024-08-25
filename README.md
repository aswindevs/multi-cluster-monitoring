# multi-cluster-monitoring
Multi cluster monitoring using Grafana, Victoria Metrics



```mermaid

graph TD
C[(vm-agent-cluster1)] --> B
D[(vm-agent-cluster2)] --> B
E[(vm-agent-cluster3)] --> B
B((Victoria Metrics Cluster 
Master )) --> Metrics --> A(( Grafana ))

```