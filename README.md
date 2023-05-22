# prompt-based-tutorial-AKS

In this tutorial, you will learn how to use Kubernetes and containers to deploy a multi-container application. You will use ChatGPT or GPT4 to guide you through a series of prompts that will help you understand the concepts and commands involved in Kubernetes. The objective of this tutorial is to simplify learning based on a prompts-enabled tutorial.

## 1st prompt : asking the copilot to act as an AKS teacher

Act as an AKS (Azure Kubernetes Service) teacher. I am an AKS learner that (is new to AKS / knowns basics of AKS, uses AKS daily and wants detailed information), i will ask you a series of questions, and you help me learn and understand by providing the best and most up to date answer, with examples and links to documentation.

## Introduction to Azure Kubernetes Service

  - What is Azure Kubernetes Service (AKS) and the benefits does it bring?

  - What are the benefits of using AKS for deploying multi-container applications?

  - How does AKS make managing and scaling containerized applications easier?

  - What is the difference between AKS and other container orchestration services?

  - How does AKS integrate with other Azure services?

  - What are some common use cases for AKS?

  - How does AKS handle security and compliance?

 - What are some best practices for getting started with AKS?
  
## Deploying your first applications on AKS

  - What are the different ways to create an AKS cluster?

  - How can I use kubectl and Azure CLI to access and manage my AKS cluster?

  - What steps should I take to prepare my application for deployment on AKS?

  - How can I use Azure Container Registry for storing and managing container images?

  - What are some common deployment strategies for applications on AKS?

  - What are the steps to run, scale, and update my application on AKS?

  - How can I use Helm charts to deploy and manage applications on my AKS cluster?

  - How can I troubleshoot common issues when deploying an application on AKS?


## End-to-end developer productivity
 - How does AKS support end-to-end developer productivity and what tools are available to improve the development workflow?
 

 - How can I use Visual Studio Code and the Kubernetes extension to develop and debug applications on my AKS cluster?

 - How can I use Azure DevOps or GitHub Actions to implement CI/CD for my applications on AKS?


## Architecture guidance and best practices for AKS
  - How to design a baseline architecture for AKS that meets your requirements and constraints?

  - How to apply best practices for cluster operators and developers for day-2 operations?

  - How to choose among different AKS solutions for specific scenarios, such as Windows containers, microservices, PCI-DSS compliance, and multiregion deployment?



## High availability
**For Developers**:

- How do I set Pod Health & Readiness Probes in AKS?
- How do Pod Disruption budgets help with high availability on AKS?

**For Admins:**

- What are some best practices for ensuring high availability on AKS?

- How do I enable Cluster availability zones on the default node pool in AKS?

- How do I design user node pools stretched on 3 AZs in AKS?

- How can I use multiple node pools to improve the availability of my applications on AKS?

- How do I use Data disks with Zonal or Regional replication (ZRS/GRS) in AKS?

- How do I use Pod anti-affinity to spread pods across nodes and zones in AKS?

- (Optional) How do I set Pod Disruption Budgets in AKS?

- How can I use load balancing and traffic routing to improve the availability of my applications on AKS?


## Scalability
**For Developers**:

- What are some best practices for ensuring scalability on AKS?

- How does AKS handle horizontal and vertical scaling of applications?

- How do I use KEDA scaler to scale workloads based on events and metrics in AKS?


**For Admins**:

- How can I use auto-scaling to automatically adjust the number of nodes and pods based on demand?

- How can I use multiple node pools to improve the scalability of my applications on AKS?

- How do I enable the KEDA addon in AKS?

- How do I enable Virtual nodes in AKS? (Note: Virtual nodes do not work with CNI Overlay)


## Networking
**For Developers**:

- How can I expose an HTTP application to external traffic using an Ingress resource in AKS?

- How can I use serviceType: clusterip to make an HTTP application accessible within the AKS cluster?

- How can I use serviceType: loadbalancer to expose a non-HTTP application externally in AKS?

- How can I use an internal load balancer with a private IP to expose a non-HTTP application within a virtual network in AKS?

**For Admins**:


- What is AZure CNI-Overlay driver for networking in AKS, and how i can use it?

- How can I use network policies to control traffic between pods in AKS?

- How can I use virtual networks and subnets to isolate and secure my AKS cluster?

- How can I use network security groups to control traffic between nodes in AKS?

- How can I force egress traffic to go through a Firewall by using the OutboundType: UDR flag during cluster creation in AKS?

- How can I set up an in-cluster Ingress controller, such as nginx, along with an External WAF like Application Gateway in AKS? (Note: Do not use AGIC for your context)

- How can I expose an HTTP application within the AKS cluster by using serviceType: clusterip?

- How can I use serviceType: loadbalancer to expose a non-HTTP application externally in AKS?

- How can I use an internal load balancer with a private IP to expose a non-HTTP application within a virtual network in AKS?




## Advanced Neworking
- How can I use a service mesh to manage traffic between microservices in AKS?

- What is Cilium and what is the difference between CNI Clilium powered Azure overlay and Azure CNI Overlay  ?
	

## Identity & RBAC
**For Developers:**

- How do I use Azure AD workload identity for App authentication & authorization in AKS?

**For Admins**:

- How do I use managed identities for cluster internal operations in AKS?

- How do I use a managed identity for the cluster server in AKS?

- (Optional) How do I use a second managed identity for kubelet in AKS?

- How do I manage Azure AD Integration for RBAC in AKS? (Note: There are 2 options for authorization: Azure RBAC or Kubernetes RBAC)

- How can I use Azure AD groups to manage access to resources in AKS?

- How do I restrict access to the API server Admin credentials in AKS? 

- How do I disable local accounts in AKS?

- How do I restrict RBAC for namespaces in AKS?

- How do I specify which teams can edit resources on a namespace and which teams have read-only access in AKS? (For example, teams belonging to Azure AD Group 1)


## Monitoring
**For Developers**:


- How do I expose health & readiness metrics for workloads/apps in AKS? (Note: Non-authenticated)


**For Admins**:

- How can I enable Diagnostic settings for a cluster in AKS?

- How can I enable container insights for a cluster in AKS?

- How can I set data collection rules to filter logs & metrics for a cluster in AKS?

- How to use Azure Monitor and Container Insights to monitor the health and performance of your cluster and applications?

- (Optional) How can I use Managed Prometheus for Metrics + managed Grafana for visualization in a cluster in AKS?

- (Optional) How can I use Prometheus alerts integration with Azure Monitor Actions (email, trigger workflow, ITSM, etc.) in a cluster in AKS?

- How can I use dashboards to visualize the health and performance of my AKS cluster and applications?

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

- How can I use encryption to secure data at rest and in transit in AKS?

- What are best practices for securing an AKS cluster?


## Cluster Upgrades
**For Developers**: None

**For Admins**:

- How can I plan and prepare for a cluster upgrade in AKS?

- How can I minimize downtime during a cluster upgrade in AKS?

- How can I roll back a cluster upgrade in AKS?

- What are some best practices for upgrading an AKS cluster?

- How do I implement blue/green deployment in AKS, for cluster upgrade?

- How do I enable cluster auto-upgrade channels in AKS?

- How do I enable patch releases for production environments in AKS?

- How do I enable stable releases for development environments in AKS?

- How do I enable node image upgrades in AKS?



## Cost Optimization
**For Developers**:


- How do I use Goldilocks for recommendations on setting CPU & RAM requests in AKS?

- How do I use affinity to reduce cross-zone charges for multi-zone clusters/pools in AKS?

**For Admins**:

- How can I use resource quotas to control the costs of my AKS cluster?

- How can I use Azure Cost Management to monitor and optimize the costs of my AKS cluster?

- How can I use Azure Advisor to get recommendations for cost optimization in AKS?

- What are some best practices for optimizing the costs of running an AKS cluster?

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


## Backup & restore
**For Developers** : 

- How do I use Infrastructure as Code in AKS?

- (Optional) How do I implement GitOps in AKS?

**For Admins**:

- How do I use Infrastructure as Code in AKS?

- (Optional) How do I implement GitOps in AKS?

- How can I use Azure Backup to protect my data on AKS?

- (Optional) How do I set Snapshot Classes for disk snapshots in AKS?

- How can I prepare for and recover from a disaster in AKS?

- What are some best practices for disaster recovery in AKS? 

- How do I restore to the same region using AKS backup in AKS? 

- How do I restore to a different region using Velero OSS in AKS? 


## Managing clusters at scale

For Both Developers and Admins:

- How can I use Azure Policy to enforce governance and compliance across multiple AKS clusters?

- How can I use Azure Monitor to monitor the health and performance of multiple AKS clusters?

- How do I manage clusters at scale using GitOps and Azure Policy in AKS?

- What are some best practices for managing multiple AKS clusters at scale?


##  Extending the capabilities of your AKS cluster
  - How to use Open Service Mesh and Dapr to add service mesh features to your applications?

  - Can you provide an example of how to use Open Service Mesh or Dapr with AKS to add service mesh features to an application?

  - How to use cluster extensions and GitHub Actions to automate and enhance your cluster operations?

  - How to use advanced networking and ingress options to connect your cluster to other Azure resources and the internet?


## Support for Linux, Windows Server, and IoT resources
 - How does AKS support Linux, Windows Server, and IoT resources?

 - What versions of Linux and Windows Server are supported by AKS?

 - How can I deploy AKS on the infrastructure of my choice using Azure Arc?

 - What are some considerations when deploying AKS on different types of infrastructure?

## Azure Kubernetes Fleet Manager
 - What is Azure Kubernetes Fleet Manager and how does it work?

 - How can I use Azure Kubernetes Fleet Manager to manage multiple AKS clusters?

 - What are the benefits of using Azure Kubernetes Fleet Manager with AKS?

## Azure Arc integration
 - How does AKS integrate with Azure Arc?

 - What is the difference between Azure Arc and Fleet Manager ?

 - How can I use Azure Arc to deploy and manage AKS clusters on-premises or at the edge?

 - What are the benefits of using AKS with Azure Arc?

## Lean more
- https://learn.microsoft.com/en-us/azure/aks/tutorial-kubernetes-deploy-application
- https://learn.microsoft.com/en-us/azure/aks/tutorial-kubernetes-prepare-app
- https://learn.microsoft.com/en-us/azure/aks/
- https://learn.microsoft.com/en-us/azure/architecture/reference-architectures/containers/aks/baseline-aks
- https://docs.microsoft.com/en-us/azure/azure-arc/
- https://docs.microsoft.com/en-us/azure/kubernetes-fleet/
- https://techcommunity.microsoft.com/t5/internet-of-things-blog/taking-azure-arc-and-kubernetes-to-the-edge/ba-p/3650599

