---
title: "Use an Application Catalog"
date: 2025-03-26
draft: false
summary: "Learn how to use an Application Catalog with Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4586873a-3df6-4457-ae53-7f1774f977f9)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-catalog)

## Details

An application catalog is a searchable software repository that you can install on an Oracle Cloud Native Environment (Oracle CNE) Kubernetes cluster. Oracle CNE supports two application catalogs: the Oracle catalog that ships with Oracle CNE and the external catalog compatible with [Artifact Hub](https://artifacthub.io/).

The Oracle catalog provides a curated selection of software supplied by Oracle. Oracle CNE ships with a built-in catalog called *embedded*. You can use the *embedded* catalog without deploying a Kubernetes cluster. The *embedded* catalog is updated when you update the `ocne` CLI.

The other catalog that ships with Oracle CNE is called the *Oracle Cloud Native Environment Application Catalog*. This catalog deploys onto your Kubernetes cluster as the *ocne-catalog* pod in the *ocne-system* namespace.

The *embedded* catalog is updated when you update the `ocne` CLI, and the Oracle Catalog is updated when you update the Kubernetes version. This behavior means the contents of the two Oracle-supplied catalogs may differ.

### Objectives

In this tutorial, you will learn:

- How to manage an Oracle-supplied catalog.
- How to install an application from an Oracle-supplied catalog.

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and one worker node
