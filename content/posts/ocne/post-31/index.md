---
title: "Deploy Oracle Cloud Native Environment User Interface"
date: 2024-06-12
draft: false
summary: "Learn how to deploy the user interface on Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/ba62a6e2-c1aa-4d39-9836-eeb49a64a56e)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-ui)

## Details

This tutorial introduces you to the new user interface features of Oracle Cloud Native Environment. The UI builds on the upstream Headlamp project that provides a fully functional Kubernetes UI.

### Objectives

In this tutorial, you will learn:

   - How to configure the Oracle Cloud Native Environment Application Catalog (Technical Preview)
   - How to install and access the Oracle Cloud Native Environment UI (Technical Preview)

### Prerequisites

- Minimum of a 3-node Oracle Cloud Native Environment cluster:

   - Operator node
   - Kubernetes control plane node
   - Kubernetes worker node

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts
   - Installation of Oracle Cloud Native Environment
