# VProfile GitOps Deployment on AWS EKS

This project demonstrates the deployment of the **VProfile application** on an **AWS EKS Kubernetes cluster** using a GitOps workflow with **Argo CD**.

The infrastructure is provisioned using **Terraform**, container images are stored in **Amazon ECR**, and application deployment is managed through **Helm and Argo CD**.

---

## Project Overview

This project includes:

- AWS EKS cluster provisioning using Terraform
- Managed EKS node group setup
- AWS Load Balancer Controller configuration
- EBS CSI Driver addon setup
- Argo CD installation using Helm
- GitOps-based application deployment
- VProfile application deployment on Kubernetes
- Public access through an ingress/domain

---

## Architecture

```text
Developer
   |
   | Push code / manifests
   v
GitHub Repository
   |
   | Sync
   v
Argo CD
   |
   | Deploys
   v
AWS EKS Cluster
   |
   | Runs
   v
VProfile Application Pods
   |
   | Exposed through
   v
AWS Load Balancer / Ingress
```

Now Let's Make a commit
