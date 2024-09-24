---
title: "Run Kubernetes"
date: 2024-09-24
draft: false
summary: "Learn to run Kubernetes on Oracle Linux using Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/01e69515-8cda-4d6e-89af-849f324c4b7f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-kube)

## Details

Kubernetes is Greek for pilot or helmsman - in other words, the person who follows commands and steers a ship towards its ultimate goal (rather than being the Captain giving orders). To that end, Kubernetes is an open-source, extensible platform for deploying, managing, and scaling containerized applications. It achieves this by using several command-line tools. This tutorial uses one of those called `kubectl` together with YAML files to define the required attributes for the organization deploying the application and understand how to set up and maintain the application once done deploying it.

All deployments onto a Kubernetes cluster get represented as objects. These deployed objects use text-based YAML files to provide details of the required state of any application deployed onto the cluster. These YAML files may describe the following:

- Which containerized applications to run on which nodes
- Details of the resources required by the application
- Any policies detailing how these applications maintain their state, such as restart policies, upgrade policies, etc.

Although essential, this third point is complicated without understanding the basics. Therefore, we'll hold off on discussing it and handle it in future tutorials.

This tutorial works with Kubernetes within an Oracle Cloud Native Environment on Oracle Linux. Its intent is not to be a 'one-stop shop' for everything needed to administer a production deployment but to introduce the necessary skills to deploy a working sample application successfully.

### Objectives

* Examine the different Kubernetes components such as a Pod, Deployment, and Service
* Examine the different Kubernetes objects
* Deploy and Test a sample project

### Prerequisites

- Installation of Oracle Cloud Native Environment