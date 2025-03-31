---
title: "Use OpenCost"
date: 2025-03-31
draft: false
summary: "Learn to install and run OpenCost on Oracle Cloud Native Environment to monitor container and cloud infrastructure costs in real-time."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/98db884c-5981-46be-ac7a-77899f102ac6)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-opencost)

## Details

Measuring the real-time costs of running and deploying applications on your Oracle Cloud Native Environment (Oracle CNE) install helps you manage them. [OpenCost](https://opencost.io/) is a vendor-neutral open-source project that records container and cloud infrastructure costs to facilitate real-time business cost monitoring. You can use the real-time costs it reports to monitor both in-cluster costs, such as CPU, GPU, and memory, and Cloud provider-based costs, such as storage.

### Objectives

In this tutorial, you will learn:

- How to install OpenCost
- How to install the OpenCost plugin using Krew
- How to use OpenCost to monitor container and cloud infrastructure costs

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
