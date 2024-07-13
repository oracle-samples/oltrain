---
title: "Manually Install on OCI"
date: 2024-01-17
draft: false
summary: "Learn to manually provision Oracle Cloud Infrastructure resources to perform an Oracle Cloud Native Environment Quick Install."
tags: ["ocne", "tutorial", "ocne-install"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-provision-oci)

## Details

Oracle Cloud Native Environment is a fully integrated suite for developing and managing cloud-native applications. The core module is the Kubernetes module. It deploys and manages containers and automatically installs and configures CRI-O, runC, and Kata Containers. CRI-O manages the container runtime for a Kubernetes cluster, which may be either runC or Kata Containers.

Oracle Cloud Native Environment Release 1.5.7 introduced the ability to use the Oracle Cloud Native Environment Platform CLI to perform a quick installation of itself. The installation runs using the `olcnectl provision` command on an installation host (the operator node). The `olcnectl provision` command can perform the following operations on the target nodes:

- Generate CA Certificates. (This tutorial uses private CA Certificates. It is recommended for a production environment that you use your own CA Certificates.)
- Copy the CA Certificates to each node.
- Set up the operating system on each node, including the network ports.
- Install the Oracle Cloud Native Environment software packages on each node.
- Start the Oracle Cloud Native Environment platform services (Platform API Server and Platform Agent).
- Create an Oracle Cloud Native Environment.
- Create, validate and install a Kubernetes module, which creates the Kubernetes cluster.
- Set up the Platform certificates to `~./olcne` on the operator node to access the environment using the `olcnectl` command.

To create more complex installation topologies, you can write your own Oracle Cloud Native Environment configuration file and then pass it to the `olcnectl provision` command using the `--config-file` option.  For more information, see the [Platform Command-Line Interface Guide](https://docs.oracle.com/en/operating-systems/olcne/1.5/olcnectl/).

### Objectives

This lab demonstrates how to:

- Create a Virtual Cloud Network (VCN) to manage resources for hosting Oracle Cloud Native Environment on OCI.
- Configure the VCN by setting up a public subnet, creating an internet gateway, making a route rule, and editing security list rules.
- Provision OCI instances to serve as operator, control, and worker nodes for Oracle Cloud Native Environment.
- Create and configure an external load balancer on OCI.
- Set up a host with the Platform CLI (_olcnectl_) on the operator node.
- Use the `olcnectl provision` command to perform a quick installation.
- Install Oracle Cloud Native Environment Release 1.8 on a five-node cluster.
- Verify the installation completed successfully.

### Prerequisites

An OCI account and a compartment in OCI.