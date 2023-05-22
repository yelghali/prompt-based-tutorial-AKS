# prompt-based-tutorial-AKS

In this tutorial, you will learn how to use Kubernetes and containers to deploy a multi-container application. You will use ChatGPT or GPT4 to guide you through a series of prompts that will help you understand the concepts and commands involved in Kubernetes. The objective of this tutorial is to simplify learning based on a prompts-enabled tutorial.

## Introduction to Azure Kubernetes Service

  - What is Azure Kubernetes Service (AKS) and its benefits?

  - What are the benefits of using AKS for deploying multi-container applications?

  - How does AKS make managing and scaling containerized applications easier?

  - What are the different ways to create an AKS cluster?

  - How can I use kubectl and Azure CLI to access and manage my AKS cluster?
  
## Deploying your first applications on AKS

  - What steps should I take to prepare my application for deployment on AKS?

  - “How can I use Azure Container Registry for storing and managing container images?

  - What are the steps to run, scale, and update my application on AKS?”

  - What is the process for upgrading Kubernetes in AKS?

Can you provide an example of how to deploy an application on AKS using Azure Container Registry?

## High availability
**For Developers**:

- How do I set Pod Health & Readiness Probes in AKS?


**For Admins:**

- How do I enable Cluster availability zones on the default node pool in AKS?

- How do I design user node pools stretched on 3 AZs in AKS?

- How do I use Data disks with Zonal or Regional replication (ZRS/GRS) in AKS?

- How do I use Pod anti-affinity to spread pods across nodes and zones in AKS?

- (Optional) How do I set Pod Disruption Budgets in AKS?


## Scalability
**For Developers**:


- How do I use KEDA scaler to scale workloads based on events and metrics in AKS?


**For Admins**:


- How do I enable cluster auto-scaler in AKS?

- How do I enable the KEDA addon in AKS?

- How do I enable Virtual nodes in AKS? (Note: Virtual nodes do not work with CNI Overlay)


## Networking
**For Developers**:

- How can I expose an HTTP application to external traffic using an Ingress resource in AKS?

- How can I use serviceType: clusterip to make an HTTP application accessible within the AKS cluster?

- How can I use serviceType: loadbalancer to expose a non-HTTP application externally in AKS?

- How can I use an internal load balancer with a private IP to expose a non-HTTP application within a virtual network in AKS?

**For Admins**:


- How can I configure the CNI-Overlay driver for networking in AKS?

- How can I force egress traffic to go through a Firewall by using the OutboundType: UDR flag during cluster creation in AKS?

- How can I set up an in-cluster Ingress controller, such as nginx, along with an External WAF like Application Gateway in AKS? (Note: Do not use AGIC for your context)

- How can I expose an HTTP application within the AKS cluster by using serviceType: clusterip?

- How can I use serviceType: loadbalancer to expose a non-HTTP application externally in AKS?

- How can I use an internal load balancer with a private IP to expose a non-HTTP application within a virtual network in AKS?



## Advanced Neworking
	- What is Cilium and what is the difference between CNI Clilium powered Azure overlay and Azure CNI Overlay  ?
	

## Identity & RBAC
**For Developers:**

- How do I use Azure AD workload identity for App authentication & authorization in AKS?

**For Admins**:

- How do I use managed identities for cluster internal operations in AKS?

- How do I use a managed identity for the cluster server in AKS?

- (Optional) How do I use a second managed identity for kubelet in AKS?

- How do I enable Azure AD Integration for RBAC in AKS? (Note: There are 2 options for authorization: Azure RBAC or Kubernetes RBAC)

- How do I restrict access to the API server Admin credentials in AKS? (Note: Restricted to a group in Azure AD)

- How do I disable local accounts in AKS?

- How do I restrict RBAC for namespaces in AKS?

- How do I specify which teams can edit resources on a namespace and which teams have read-only access in AKS? (For example, teams belonging to Azure AD Group 1)


## Monitoring
**For Developers**:


- How do I expose health & readiness metrics for workloads/apps in AKS? (Note: Non-authenticated)


**For Admins**:

- How do I enable Diagnostic settings for a cluster in AKS?

- How do I enable container insights for a cluster in AKS?

- How do I set data collection rules to filter logs & metrics for a cluster in AKS?

- How to use Azure Monitor and Container Insights to monitor the health and performance of your cluster and applications?

- (Optional) How do I use Managed Prometheus for Metrics + managed Grafana for visualization in a cluster in AKS?

- (Optional) How do I use Prometheus alerts integration with Azure Monitor Actions (email, trigger workflow, ITSM, etc.) in a cluster in AKS?

- how to optimize the costs of monitoring AKS on Azure ?


## Security
**For Developers:**


- How do I scan container images in AKS?

- How do I secure access to the container registry in AKS?

- how to manage workload identities on AKS ?

- how to provide my workload access to the Key vault on AKS ?

**For Admins**:

- How do I set network policies at the namespace level in AKS? (Note: Deny all by default)

- How do I enable a private cluster in AKS?

- How do I enable Azure Policies in AKS?

- How do I enable Defender in AKS?

- How do I enable monitoring in AKS?

- How do I enable Key Vault CSI Integration in AKS?

- How do I enable the secret store CSI driver in AKS?

- How do I enable Azure AD Integration in AKS?

- How do I secure Ingress traffic with a Web Application Firewall (WAF) in AKS?

- How do I secure egress traffic through Azure Firewall or NVA in AKS?

- How do I scan container images in AKS?

- How do I secure access to the container registry in AKS?

- What are best practices for securing an AKS cluster?

## Cluster Upgrades
**For Developers**: None

**For Admins**:


- How do I enable cluster auto-upgrade channels in AKS?

- How do I enable patch releases for production environments in AKS?

- How do I enable stable releases for development environments in AKS?

- How do I enable node image upgrades in AKS?

- How do I enable the Image Cleaner in AKS?

- How do I implement blue/green deployment in AKS?


## Cost Optimization
**For Developers**:


- How do I use Goldilocks for recommendations on setting CPU & RAM requests in AKS?

- How do I use affinity to reduce cross-zone charges for multi-zone clusters/pools in AKS?

**For Admins**:


- How do I use the Cluster Autoscaler in AKS? (Note: The biggest chunk of savings is here)

- How do I use the Start/Stop feature for development environments in AKS?

- How do I use dedicated Node Pools for special workloads in AKS?

- How do I use Spot instances in AKS?

- How do I use Reserved Instances in AKS?

- How do I use Burstable VMs in AKS?

- When to use Spot VM, reserved instances and bustable VMS ?

- How do I use Goldilocks for recommendations on setting CPU & RAM requests in AKS?

- How do I use affinity to reduce cross-zone charges for multi-zone clusters/pools in AKS?

- How do I use ACI through virtual nodes in AKS?


## Resiliency of compute and data

 - How does AKS ensure the resiliency of compute and data?*
 
 - What features and tools are available in AKS to improve the resiliency of my applications?

 - What are some best practices for ensuring the resiliency of compute and data in AKS?


## Backup & restore
**For Developers** : 

- How do I use Infrastructure as Code in AKS?

- (Optional) How do I implement GitOps in AKS?

**For Admins**:

- How do I use Infrastructure as Code in AKS?

- (Optional) How do I implement GitOps in AKS?

- How do I enable AKS backup for disks in AKS?

- How do I enable Azure backup for Fileshare in AKS?

- How do I enable Azure Blob replication for blobs in AKS?

- (Optional) How do I set Snapshot Classes for disk snapshots in AKS?

- How can I prepare for and recover from a disaster in AKS?

- What are some best practices for disaster recovery in AKS? 

- How do I restore to the same region using AKS backup in AKS? 

- How do I restore to a different region using Velero OSS in AKS? 


## Managing clusters at scale

For Both Developers and Admins:

- How do I manage clusters at scale using GitOps and Azure Policy in AKS?


## Architecture guidance and best practices for AKS
  - How to design a baseline architecture for AKS that meets your requirements and constraints?
  - How to apply best practices for cluster operators and developers for day-2 operations?
  - How to choose among different AKS solutions for specific scenarios, such as Windows containers, microservices, PCI-DSS compliance, and multiregion deployment?


##  Extending the capabilities of your AKS cluster
  - How to use Open Service Mesh and Dapr to add service mesh features to your applications?
  - Can you provide an example of how to use Open Service Mesh or Dapr with AKS to add service mesh features to an application?
  - How to use cluster extensions and GitHub Actions to automate and enhance your cluster operations?
  - How to use advanced networking and ingress options to connect your cluster to other Azure resources and the internet?


## Automated management and scalability
 - What is automated management and scalability in AKS?
 - How does AKS provide enterprise-grade container orchestration?
 - How can I use automated management and scalability to improve my AKS cluster operations?

## End-to-end developer productivity
 -How does AKS support end-to-end developer productivity and what tools are available to improve the development workflow?
 - What tools and features are available in AKS for debugging, CI/CD, logging, and automated node maintenance?
 - How can I use these tools and features to improve my development workflow with AKS?

## Support for Linux, Windows Server, and IoT resources
 - How does AKS support Linux, Windows Server, and IoT resources?
 - How can I deploy AKS on the infrastructure of my choice using Azure Arc?
 - What are some considerations when deploying AKS on different types of infrastructure?

## Azure Kubernetes Fleet Manager
 - What is Azure Kubernetes Fleet Manager and how does it work?
 - How can I use Azure Kubernetes Fleet Manager to manage multiple AKS clusters?
 - What are the benefits of using Azure Kubernetes Fleet Manager with AKS?

## Azure Arc integration
 - How does AKS integrate with Azure Arc?
 - How can I use Azure Arc to deploy and manage AKS clusters on-premises or at the edge?
 - What are the benefits of using AKS with Azure Arc?

## Lean more
- https://learn.microsoft.com/en-us/azure/aks/tutorial-kubernetes-deploy-application
- https://learn.microsoft.com/en-us/azure/aks/tutorial-kubernetes-prepare-app
- https://learn.microsoft.com/en-us/azure/aks/
- https://learn.microsoft.com/en-us/azure/architecture/reference-architectures/containers/aks/baseline-aks

