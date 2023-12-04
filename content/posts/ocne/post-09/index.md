---
title: "Compact Deployment"
date: 2022-06-30
draft: false
summary: "The 1.5 release of Oracle Cloud Native Environment introduced the compact deployment, allowing non-system Kubernetes workloads to run on control plane nodes."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/c1bf32f7-7809-4355-bf83-d3f46797dd02)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-compact)

## Details

The 1.5 release of Oracle Cloud Native Environment introduced the compact deployment, allowing non-system Kubernetes workloads to run on control plane nodes. When setting `--compact` to `true`, the Platform API Server does not taint the control plane node(s). This setting allows non-system Kubernetes workloads to be scheduled and run on control plane nodes.

> **Important:** This option must be set to false (the default) for production environments.

During this tutorial, you create, validate, and install a compact Oracle Cloud Native Environment deployment.

### Objectives

At the end of this tutorial, you should be able to do the following:

- Create a compact deployment
- Verify deployment with a test project

### Prerequisites

The tutorial uses the following system:

- A single Oracle Linux instance provisioned with the following:
  - a non-root user with sudo permissions
