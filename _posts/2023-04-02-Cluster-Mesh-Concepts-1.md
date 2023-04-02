---
title: "Cluster Mesh - Concepts"
date: 2023-01-20
---
# Cluster Mesh
@kubernetes 

Clusters in enterprises are similar to private cars in cities. A cluster typically belongs to a line of business, a department, a team -  usually an entity that is capable of justifying the need of kubernetes and microservices. Often, there is no rationlization of the cluster capacity utilization and leveraging software assets deployed on a cluster. This often leads to underutilized cluster of capacity - s as well as common software. This issue is not limited to just the dev/test environments, but becomes more severe in automated workload placement -  neccessitate a redundant secondary using lesser utilization. Without careful planning, utilizing the resources is never easy.   
Some of the well-known patterns to address this challenge of fragmented capacity as well as reducing passive capacity includes:
+ abstraction of capacity - addressing capacity as a single logical construct spread over multiple clusters
+ automated workload placement -  workload placement on the clusters using intellegent tools that dynamically decide the deployment targets based on the utilization of cluster resources
+ federation of capacity - providing the ability to spread the components of the applications on different clusters which can then communicate with each other.


## Key Concepts
1. Cluster  - a kubernetes cluster
2. Fleet    - a set of kubernetes clusters that are interconnected and can communicate with each other
3. Workload - an application that can be deployed on a kubernetes cluster


## Cluster Mesh

A [cluster mesh](images/cluster-mesh.png) is formed by integrating together multiple kubernetes clusters.    
For e.g.

![images/cluster-mesh.png](https://github.com/adventuresincode/blog/blob/main/_posts/images/cluster-mesh.png)

