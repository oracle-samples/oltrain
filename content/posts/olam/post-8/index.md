---
title: "Manage KVM Virtual Machines"
date: 2024-12-20
draft: false
summary: "Learn how to use the libvirt community collection to manage KVM virtual machines with Oracle Linux Automation Manager."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/3e869b97-6f71-46fa-a979-e0c8bf81d7d2)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-libvirt-collection)

## Details

The *community.libvirt* collection provides libvirt modules and plugins supported by the Ansible libvirt community. These modules and plugins help manage virtual machines (VMs) and containers using the [libvirt](https://libvirt.org/) API.

### Objectives

In this tutorial, you'll learn how to:

- Create a playbook that uses the *community.libvirt* collection
- Configure credentials for Ansible Galaxy
- Create a Job Template
- Run the Job

### Prerequisites

- A system with Oracle Linux Automation Manager installed
- Access to a Git repository
- An Oracle Linux system with KVM installed
