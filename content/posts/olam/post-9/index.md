---
title: "Setup HAProxy as Load Balancer"
date: 2023-05-06
draft: false
summary: "Learn how to configure HAProxy to Load Balance an Oracle Linux Automation Manager Cluster."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/1d19c310-b6d6-40a9-aa2b-44dee29a8f31)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-haproxy-cluster)

## Details

Oracle Linux Automation Manager supports a cluster deployment of multiple control and execution nodes. With the control nodes acting as the entry point into the cluster, how does an administrator manage the traffic across these nodes? That is where a load balancer becomes beneficial. A load balancer efficiently distributes incoming network traffic across a group of backend servers or, in this solution, the control nodes. A load balancer ensures the Oracle Linux Automation Manager infrastructure is highly available and reliable, and performance does not degrade.

The sample inventory below defines a multi-node cluster deployment in the free lab environment. To help automate the cluster installation on your hardware, check out the playbook in the [Oracle Linux Automation Manager](https://https://github.com/oracle-samples/ansible-playbooks/tree/main/playbooks/OLAM/cluster-plus-hop-node) section of the [ansible-playbooks](https://github.com/oracle-samples/ansible-playbooks) project.

This sample inventory creates a cluster of three control plane nodes, two execution nodes, and a remote database.

![playbook-inv](./images/playbook-inv.png " ")

This image shows the topology for this cluster.

![topology](./images/topology.png " ")

Although there are many load balancer options, this tutorial will leverage HAProxy. HAProxy, or High Availability Proxy, is an application layer (Layer 7) load balancer and high-availability solution that you can use to implement a reverse proxy for HTTP and TCP-based Internet services. An application layer load balancer often includes many features because it can inspect the traffic content it is routing and either modify content within each packet or make decisions about handling each packet based on its content. These features simplify implementing session persistence, TLS, ACLs, and HTTP rewrites and redirection.

### Objectives

In this tutorial, you'll learn how to:

- Install HAProxy
- Configure HAProxy
- Configure Oracle Linux Automation Manager to work behind a load balancer or proxy

### Prerequisites

- A cluster with Oracle Linux Automation Manager installed and cluster configured
- An Oracle Cloud Infrastructure (OCI) account
- A user in the OCI account with permission to work with resources in a compartment
- Access to that account's credentials and OCID information
  
  For details on installing Oracle Linux Automation Manager, see the [Oracle Linux Automation Manager Installation Guide](https://docs.oracle.com/en/operating-systems/oracle-linux-automation-manager/).
