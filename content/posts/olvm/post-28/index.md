---
title: "Install on OCI"
date: 2025-03-04
draft: false
summary: "Learn to deploy Oracle Linux Virtualization Manager in Oracle Cloud Infrastructure."
tags: ["olvm", "lab","tutorial","olvm-deploy"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/c912c867-a5cd-420e-9ee5-ee9017b2b957)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olvm-install)

## Details

Oracle Linux Virtualization Manager is a server virtualization management platform that you can deploy to configure, monitor, and manage an Oracle Linux Kernel-based Virtual Machine (KVM) environment with enterprise-grade performance and support from Oracle.

This tutorial provides a guide for installing a working and functional deployment of Oracle Linux Virtualization Manager on Oracle Cloud Infrastructure (OCI).

> **Note:** This tutorial is only for testing and evaluation purposes; Oracle Linux Virtualization Manager support for OCI is under development and is not supported to manage OCI systems.

### Objectives

In this tutorial, you'll learn how to:

- Deploy the underlying OCI virtual cloud network (VCN) and instances
- Install Oracle Linux Virtualization Manager engine
- Attach a KVM host
- Attach shared storage
- Import an OVA template
- Create a new virtual machine

### Prerequisites

- Access to an OCI tenancy
- A new VCN (10.0.0.0/16) with these resources:
  - One public subnet (10.0.0.0/24) for the primary VNIC on the hosted engine and Oracle Linux Kernel-based Virtual Machine (KVM) hosts
  - One private subnet (10.0.1.0/24) for the secondary VNIC on the hosted engine and KVM hosts
  - One Virtual Local Area Network (VLAN) 1 (10.0.10.0/24) for the KVM hosts virtual machines
  - One Internet Gateway
  - One Service Gateway
  - One public route table (0.0.0.0/0 through Internet Gateway) and associate it with the public subnet and VLAN 1
  - One private route table (ALL through Service Gateway) and associate it with the private subnet
  - Security lists should allow:
    - All egress connections (0.0.0.0/0) all protocols
    - All ingress connections from VCN CIDR (10.0.0.0/16)
    - Ingress connection for all protocols from client PC

- Two 1TB block storage volumes
- Create one VM instance (recommended configuration: VM.Standard.E5.Flex with 2 OCPUs/32GB RAM) running Oracle Linux for the hosted engine. Attach a secondary VNIC to the VM instance and connect it to the private subnet.
- Create two VM instances (recommended configuration: VM.Standard.E5.Flex with 8 OCPUs/64GB RAM) running Oracle Linux to use as KVM hosts. Attach two secondary VNICs to each VM host and connect them to the private subnet and the VLAN. Attach two block volumes to each as read-write and shareable.
