---
title: "Install OCI Cluster"
date: 2024-10-30
draft: false
summary: "Learn to use the oci provider to deploy and manage Oracle Cloud Native Environment on Oracle Cloud Infrastructure."
tags: ["ocne2", "lab", "tutorial", "ocne2-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/e233c434-9d07-44f5-bf6a-6bf1314f8a00)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-install-oci)

## Details

Oracle Cloud Native Environment includes a Command Line Interface (CLI) that can manage the life cycle of Kubernetes clusters using OSTree-based container images. Oracle Cloud Native Environment includes several provider types you can use to create a Kubernetes cluster, and this tutorial introduces how to use the `ocne cluster` command to deploy a Kubernetes cluster to Oracle Cloud Infrastructure using the *oci* provider.

Creating a cluster on Oracle Cloud Infrastructure requires you to provide details of an existing tenancy and have all the necessary privileges to create and destroy compute instances. The *oci* provider requires a compartment that is available to use. The Compartment can be specified by referencing its Oracle Cloud Identifier (OCID) or its path in the compartment hierarchy.

For more information about Oracle Cloud Native Environment 2, please refer to the current [Release Documentation](https://docs.oracle.com/en/operating-systems/olcne/).

### Objectives

In this tutorial, you'll learn to:

- Install the prerequisites for the *oci* provider
- Use the *oci* provider to create and manage a Kubernetes cluster

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts

- OCI cluster creation requires access to the following resources in an Oracle Cloud Infrastructure tenancy:

  - Virtual cloud network with four subnets
  - Network load balancer
  - Object Storage bucket with minimum 5 GiB available
  - Compute Custom Image
  - Compute Arm Shape for the control plane node
    - VM.Standard.A1.Flex with two OCPU and 12 memory
  - Compute for each additional control plane and worker node
    - VM.Standard.E4.Flex with four OCPU and 64 memory