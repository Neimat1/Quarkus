# Quarkus

  Today, big data does not merely mean a big quantity of datasets but flexible storage options for a big quantity of data.

This is where containers and, specifically, Kubernetes fits in. In a nutshell, you can think of a container as a packaged application that contains just the libraries that are needed to run it, and Kubernetes is like an orchestrating system that makes sure all the containers have the appropriate resources while managing their life cycle.

Kubernetes runs images and manages containers using Docker.

**Kubernetes**: focuesd around 
  + The concept of loosely coupled
  + Flexible mechanism for service discovery
 
### Kubernets Components
![image](https://user-images.githubusercontent.com/63751555/223565727-db6f1fd4-af6d-4857-bf56-0a022b5261c5.png)
  
 + **Master Node**: make up brain for cluster, responsible for managing overall the cluster
   + API server: Synchronize and validate information running in pods
   + etcd: provides consistent and hight availablity storage for cluster data 
   + Controller Manager: check changes in **etcd** and uses its api to enforce the desired state 
   + HA Proxy:we add when we configuring the HA master to balance load between severel master endpoints
 + **Nodes**: conatin all services that are needed to run the applcations in commponents called pods. Each node exposes a set of resources (such as computing, networking, and storage) to your applications. run as a VM.
   + Pods: group conatiners and pieces of application together
   + Kubelet: agent runs in each node and makes sure that containers running in a pod
   + Kube-Proxy: maintains network rules on node
   + Container runtime: software responsible for running containers
### Kubernets benefits
  + Simplifies container management
  + Speed up the process of testing, releasing and building
  + Provides fastest and least costly horizonetal scalability
  + Manage stateless and stateful applications

## Good refernces
  - https://github.com/PacktPublishing/Hands-On-Cloud-Native-Applications-with-Java-and-Quarkus
  
