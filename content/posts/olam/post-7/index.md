---
title: "Use Hop Nodes"
date: 2023-03-10
draft: false
summary: "Learn how to use a hop node in Oracle Linux Automation Manager."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/c4780f15-bd17-468d-9133-3eba9bc0ff2a)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-hop-node)

## Details

Oracle Linux Automation Manage supports a service mesh technology based on the upstream [receptor](https://receptor.readthedocs.io/en/latest/) project. The service mesh links controller, hop, and execution nodes into an overlay network through a daemon-based receptor application.

Oracle Linux Automation Manager introduces the hop node as part of the service mesh. This node type allows relaying tasks from control plane nodes to execution nodes on remote or restricted networks in the same way SSH uses a jump host. This implementation enables running jobs across different execution nodes and moving tasks closer to the systems needing automation.

These guides show several methods to check the status of a service mesh and confirm the topology communication between the various nodes.

### Objectives

In this lab, you'll learn how to:

  - List the capacity of the control plane and execution nodes
  - View the Service Mesh status for a given cluster node
  - View the Service Mesh status using an API call

### Prerequisites

  - A cluster with Oracle Linux Automation Manager installed and Service Mesh configured
  - An Oracle Cloud Infrastructure (OCI) account
  - A user in the OCI account with permission to work with resources in a compartment
  - Access to that accounts credentials and OCID information

