# Bootstrapping k0s cluster on Hetzner

This directory provides an example flow with `k0sctl` tool together with Terraform using Hetzner as the cloud provider.

## Prerequisites
- You need an account and API token for Hetzner
- Terraform installed

## Steps
Create terraform.tfvars file with needed details. You can use the provided terraform.tfvars.example as a baseline.
- terraform init
- terraform apply
- terraform output k0s_cluster > k0sctl.yaml
- k0sctl apply
- Optional: k0sctl kubeconfig > ~/.kube/config