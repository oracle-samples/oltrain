---
title: "How to Upgrade to Oracle Cloud Native Environment"
date: 2023-04-13
draft: false
summary: "This tutorial will show how to upgrade an Oracle Cloud Native Environment Release 1.6 install to Release 1.7."
tags: ["ocne", "lab", "tutorial"]
showDate: true
---

## Links

:crescent_moon: [How to Upgrade to Oracle Cloud Native Environment](https://luna.oracle.com/lab/fa8fc61b-893c-4507-93a2-711540e9ace7)

:spiral_notepad: [How to Upgrade to Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-upgrade)

## Details

Administrators of an Oracle Cloud Native Environment deployment are aware that many of the components, such as Kubernetes, are regularly updated.  The upgrade process updates these components to the most recent release allowing any new features to become available for users.

This tutorial will show how to upgrade an Oracle Cloud Native Environment Release 1.6 install to Release 1.7.

> **Note:** Please note that Oracle Cloud Native Environment upgrades are incremental and not cumulative.  This is due to a limitation from both the Kubernetes and Istio modules which require incremental upgrades.

### Objectives

In this tutorial, you will learn how to:

- Upgrade an Oracle Cloud Native Environment install from Release 1.6 to Release 1.7.

### Prerequisites

- 3 Oracle Linux systems to use as:
  - Operator node (ocne-operator)
  - Kubernetes control plane node (ocne-control)
  - Kubernetes worker node (ocne-worker)

- Each system should have the latest Oracle Linux 8 (x86_64) installed

- This environment is pre-configured with:
  - An oracle user account (used during the install) with sudo access
  - Key-based SSH, also known as passwordless SSH, between the hosts
  - Installation of Oracle Cloud Native Environment and CCM module
