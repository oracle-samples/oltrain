---
title: "Use Quick Install to Deploy Oracle Cloud Native Environment"
date: 2022-11-28
draft: false
summary: "Oracle Cloud Native Environment Release 1.5.7 introduced the ability to use the Oracle Cloud Native Environment Platform CLI to perform a quick installation of itself. This is done using the olcnectl provision command on an installation host (the _operator_ node)."
tags: ["ocne", "lab", "tutorial"]
showDate: true
---

## Links

:crescent_moon: [Use Quick Install to Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/42f9b19b-e254-42cf-885d-a80127d9d751)

:spiral_notepad: [Use Quick Install to Deploy Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-quick-install)

## Details

Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications.  The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers.  CRI-O manages the container runtime for a Kubernetes cluster.  The runtime may be either runC or Kata Containers.

Oracle Cloud Native Environment Release 1.5.7 introduced the ability to use the Oracle Cloud Native Environment Platform CLI to perform a quick installation of itself. This is done using the _olcnectl provision_ command on an installation host (the _operator_ node).  The _olcnectl provision_ command can perform the following operations on the target nodes:

- Generate CA Certificates.
- Copy the CA Certificates to each node.
- Set up the operating system on each node, including the network ports.
- Install the Oracle Cloud Native Environment software packages on each node.
- Start the Oracle Cloud Native Environment platform services (Platform API Server and Platform Agent).
- Create an Oracle Cloud Native Environment.
- Create, validate and install a Kubernetes module, which creates the Kubernetes cluster.
- Set up the Platform certificates to `~./olcne` on the operator node to access the environment using the _olcnectl_ command.

This tutorial describes how to perform a quick installation using the simplest series of steps possible to get Oracle Cloud Native Environment and a Kubernetes cluster installed. This tutorial uses private CA Certificates. It is recommended for a production environment that you use your own CA Certificates.
More complex install topologies can be achieved by writing your own Oracle Cloud Native Environment configuration file and then passing it to the _olcnectl provision_ command using the _--config-file_ option.  For more information on the syntax options provided by the _olcnectl provision_ command and also on how to write a configuration file, please refer to the [Platform Command-Line Interface](https://docs.oracle.com/en/operating-systems/olcne/1.5/olcnectl/) guide.

### Objectives

In this tutorial, you will learn how to:

- Perform a quick installation of Oracle Cloud Native Environment
- Set up a host with the Platform CLI (olcnectl) on the operator node
- Use the olcnectl provision command to perform a quick installation
- Install Oracle Cloud Native Environment Release 1.7 on a 3-node cluster
- Verify the install completed successfully

### Prerequisites

The host systems to perform the steps in this tutorial are listed in this section. To be successful requires:

- 3 Oracle Linux systems to use as:
  - Operator node (ocne-operator)
  - Kubernetes control plane node (ocne-control)
  - Kubernetes worker node (ocne-worker)

- Each system should have a minimum of the following installed:
  - Latest Oracle Linux (x86_64) installed and running the Unbreakable Enterprise Kernel Release 7 (UEK R7)

- This environment is pre-configured with:
  - An oracle user account (used during the install) with sudo access
  - Key-based SSH, also known as passwordless SSH, between the hosts
