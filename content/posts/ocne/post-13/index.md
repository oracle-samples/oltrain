---
title: "Use OCI Cloud Controller Manager"
date: 2022-08-26
draft: false
summary: "Learn how to enable the LoadBalancer Service type in Oracle Cloud Native Environment on Oracle Cloud Infrastructure."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5571f277-3eb9-435f-b3b3-fe421fb9747e)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-loadbalancer)

## Details

The Kubernetes [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) Service exposes the Deployment externally using a cloud provider's load balancer. The dependent NodePort and ClusterIP Services, to which the external load balancer routes, are automatically created.

This tutorial shows how to deploy the Oracle Cloud Infrastructure Cloud Controller Manager module (OCI-CCM module) within Oracle Cloud Native Environment to handle requests for an external LoadBalancer Service type. The Oracle Cloud Infrastructure Cloud Controller Manager module uses the open source [oci-cloud-controller-manager](https://github.com/oracle/oci-cloud-controller-manager) project, which is a Kubernetes Cloud Controller Manager implementation (or out-of-tree cloud-provider) for Oracle Cloud Infrastructure (OCI).

### Objectives

At the end of this tutorial, you should be able to do the following:

- Deploy the Oracle Cloud Infrastructure Cloud Controller Manager module
- Create a Deployment and LoadBalancer Service
- Verify access through the LoadBalancer Service

### Prerequisites

An Oracle Linux instance with the following configuration:

- a non-root user with sudo privileges
- Oracle Cloud Native Environment installed and configured
