---
title: "Enable Istio Proxy Sidecar Injection"
date: 2022-09-21
draft: false
summary: "Istio is a Service Mesh that provides a separate infrastructure layer to handle inter-service communication. Network communication is abstracted from the services themselves and handled by proxies. Istio uses a sidecar design, which means that communication proxies run in their own containers beside every service container."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6e667326-fd72-4e65-a5b5-8398c5eef960)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-sidecars/)

## Details

Istio is a service mesh that provides a separate infrastructure layer to handle inter-service communication. Network communication is abstracted from the services themselves and handled by proxies. Istio uses a sidecar design, which means that communication proxies run in their own containers beside every service container. To put Istio automatic sidecar injection into effect, the namespace to be used by an application must be labeled with `istio-injection=enabled`.
This tutorial uses an existing Highly Available Kubernetes cluster running on Oracle Cloud Native Environment, and has the following modules deployed:

- Kubernetes (`kubernetes`)
- Oracle Cloud Infrastructure Cloud Controller Manager Module (`oci-ccm`)

The starting deployment consists of the following:

- 1 Operator Node
- 3 Control Plane Nodes
- 5 Worker Nodes

It builds upon the labs:

- [Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/d18fe294-efb5-4498-9e7b-d5cc724d8619/steps)
- [Deploy an External Load Balancer with Oracle Cloud Native Environment](https://luna.oracle.com/lab/be8d99fc-44c3-4062-a3c3-95e982243ccf/steps)
- [Use OCI Cloud Controller Manager on Oracle Cloud Native Environment](https://luna.oracle.com/lab/5571f277-3eb9-435f-b3b3-fe421fb9747e/steps)

### Objectives

This tutorial/lab shows how to install Istio and then enable automatic proxy sidecar injection, and thus take advantage of Istio's features in Oracle Cloud Native Environment.

The following steps will be outlined:

- Install the Istio module.
- Deploy an application without automatic proxy sidecar injection enabled.
- Remove the deployment.
- Enable automatic proxy sidecar injection.
- Deploy the same application again - notice that the pods in the service mesh are executing with an associated Istio sidecar proxy.

### Prerequisites

> **Note:** If using the free lab environment these prerequisites are provided as the starting point.

- Systems should have:
  - A minimum of latest Oracle Linux 8 (x86_64) installed and running the Unbreakable Enterprise Kernel Release 6 (UEK R6).
  - Completed the [prerequisite steps to install Oracle Cloud Native Environment](https://docs.oracle.com/en/operating-systems/olcne/1.5/start/prereq.html#prereq).
  - The Istio module already configured. For more information on deploying the Istio module, see the [Oracle Cloud Native Environment Documentation](https://docs.oracle.com/en/operating-systems/olcne/1.5/mesh/).
