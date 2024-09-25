---
title: "Introducing Kubectl"
date: 2024-09-26
draft: false
summary: "Learn how to use kubectl with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6c65a513-b161-47d2-b45c-92ca02e38dc0)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-kubectl-intro)

## Details

Although graphical tools can manage Kubernetes, many administrators prefer to use command-line tools. The command line tool provided within the Kubernetes ecosystem is called [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/). Kubectl is a versatile tool used to deploy and inspect the configurations and logs of the cluster resources and applications. Kubectl achieves this by using the Kubernetes API to authenticate with the Control Node of the Kubernetes cluster to complete any management actions requested by the administrator. 

Most of the operations/commands available for kubectl provide administrators with the ability to deploy and manage applications deployed onto the Kubernetes cluster and inspect and manage the Kubernetes cluster resources. Because this tutorial is an introduction to kubectl, it will only focus on using kubectl to discover what Kubernetes resources are available in a new install of Oracle Cloud Native Environment.

> **Note:** Many kubectl commands have the `--all-namespaces` option appended. For this reason, a shorthand for this option is the `-A` flag. This tutorial often uses `kubectl -A` instead of `kubectl --all-namespaces`.

### Objectives

This tutorial introduces kubectl, a widely used command-line tool for interacting with a Kubernetes cluster. Beginning with why it is helpful to learn about it, the tutorial will also introduce some basic kubectl commands that help to understand any services deployed on a Kubernetes cluster, for example:

   - location of the configuration file
   - _kubectl config_
   - _kubectl get_
   - _kubectl describe_
   - _kubectl version_

Most of these commands provide both _getter_ (to review settings) and _setter_ (to define/update settings) functions. This tutorial only uses kubectl to view the current configuration information.

### Prerequisites

- Installation of Oracle Cloud Native Environment
