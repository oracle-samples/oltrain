---
title: "Backup Control Plane Nodes"
date: 2024-04-26
draft: false
summary: "Learn to backup, restore, and inspect a control plane backup for Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6055f3b0-aed4-443e-829a-6d3825b0507d)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-cp-backup)

## Details

Oracle Cloud Native Environment ships with a module that allows an administrator to back up and restore the control plane configuration files. This tutorial covers performing a backup, inspecting the backup file, and then restoring from the backup file.

### Objectives

In this lab, you'll learn how to:

- Back up a control plane configuration
- Inspect the backup file
- Restore the backup file

### Prerequisites

- Minimum of a 3-node Oracle Cloud Native Environment cluster:

   - Operator node
   - Kubernetes control plane node
   - Kubernetes worker node

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts
   - Installation of Oracle Cloud Native Environment
