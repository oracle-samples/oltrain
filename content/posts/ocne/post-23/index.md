---
title: "Use Persistent Volumes and Persistent Volume Claims"
date: 2023-11-15
draft: false
summary: "This tutorial shows how to create and use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial"]
showDate: true
---

## Links

:crescent_moon: [Use Persistent Volumes and Persistent Volume Claims](https://luna.oracle.com/lab/cdf43182-16c7-4c42-9a91-6052a5934184)

:spiral_notepad: [Use Persistent Volumes and Persistent Volume Claims](https://docs.oracle.com/en/learn/ocne-pv/#introduction)

## Details

This tutorial shows how to create and use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment. Both Persistent Volumes and Persistent Volume Claims work together to provide persistence to any container-based applications deployed onto Oracle Cloud Native Environment. You will start by covering how to use Persistent Volumes initially, and then cover the use of Persistent Volume Claims.

### Objectives

You will learn:

- The difference between a Persistent Volume (PV) and a Persistent Volume Claim (PVC)
- How to use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment.

### Prerequisites

- 3 Oracle Linux systems to use as:
	- Operator node (ocne-operator-01)
	- Kubernetes control plane node (ocne-control-01)
	- Kubernetes worker node (ocne-worker-01)

- Each system should have the latest Oracle Linux 8 (x86_64) installed

- This environment is pre-configured with:
    - An Oracle user account (used during the installation) with sudo access
	- Key-based SSH, also known as password-less SSH, between the hosts
	- Installation of Oracle Cloud Native Environment and Oracle Cloud Infrastructure Cloud Controller Manager (oci-ccm) module
