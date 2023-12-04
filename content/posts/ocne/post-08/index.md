---
title: "Run Kubernetes on Oracle Linux"
date: 2022-06-30
draft: false
summary: "This tutorial works with Kubernetes running within a compact Oracle Cloud Native Environment on Oracle Linux. It introduces the skills required to deploy a working sample application."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Run Kubernetes on Oracle Linux](https://luna.oracle.com/lab/01e69515-8cda-4d6e-89af-849f324c4b7f)

:spiral_notepad: [Run Kubernetes on Oracle Linux](https://docs.oracle.com/en/learn/ol-kube)

## Details

Kubernetes is Greek for pilot or helmsman - in other words, the person who follows commands and steers a ship towards its ultimate goal (rather than being the Captain giving orders). To that end, Kubernetes is an open-source, extensible platform for deploying, managing, and scaling containerized applications. It achieves this by using several command-line tools. This lab uses one of those called kubectl together with YAML files to define the required attributes for the organization deploying the application and understand how to set up and maintain the application once done deploying it.

All deployments onto a Kubernetes cluster get represented as objects. These deployed objects use text-based YAML files to provide details of the required state of any application deployed onto the cluster. These YAML files may describe the following:

- Which containerized applications to run on which nodes
- Details of the resources required by the application
- Any policies detailing how these applications maintain their state, such as restart policies, upgrade policies, etc.

This third point, although important, is complicated without understanding the basics. Therefore, we'll hold off for now and handle that topic in future tutorials.
This tutorial works with Kubernetes running within a compact Oracle Cloud Native Environment on Oracle Linux. The intent is not to be a 'one stop shop' for everything needed to administer a production deployment. Instead, it introduces the skills required to deploy a working sample application.

### Objectives

At the end of this tutorial, you should be able to do the following:

- Examine the different Kubernetes components such as a Pod, Deployment, and Service
- Examine the different Kubernetes objects
- Deploy and Test a sample project

### Prerequisites

The tutorial uses the following system:

An Oracle Linux 8 or later system with the following configuration:

- a non-root user with sudo privileges
- Oracle Cloud Native Environment installed and configured
