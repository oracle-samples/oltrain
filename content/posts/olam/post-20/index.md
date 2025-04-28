---
title: "Use virt-v2v"
date: 2024-08-27
draft: false
summary: "Learn to automate the conversion of existing virtual machines using virt-v2v with Oracle Linux Automation Manager."
tags: ["olam","tutorial"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-virt-v2v/)

## Details

Oracle Linux Virtualization Manager is a server virtualization management platform you can easily deploy to configure, monitor, and manage an Oracle Linux Kernel-based Virtual Machine (KVM) environment. If you are already leveraging other virtualization solutions like VMware and are interested in migrating existing virtual machines from a VMware environment to Oracle Linux Virtualization Manager, a tool named `virt-v2v` can be used.

You can combine the `virt-v2v` tool with Oracle's automation solution, Oracle Linux Automation Manager. It helps minimize the need for human intervention during migrations.

Let's explore and demonstrate how to automate the migration of existing VMs running in a VMware environment to Oracle Linux Virtualization Manager using Oracle Linux Automation Manager.

### Objectives

In this tutorial, you'll learn how to:

- Create Surveys in Oracle Linux Automation Manager
- Automate the migration of VMs to Oracle Linux Virtualization Manager using Oracle Linux Automation Manager

### Prerequisites

- A system with Oracle Linux Automation Manager installed
- Existing Oracle Linux Virtualization Manager Environment
- The Oracle Linux Automation Manager Machine should be able to connect using SSH to the VMware and Oracle Linux Virtualization Manager environments
- You need to download and transfer the VMware Virtual Disk Development Libraries (VDDK) to the KVM Host as per the instructions in the [blog](https://blogs.oracle.com/linux/post/oracle-linux-virtualization-manager-importing-virtual-machines-from-vcenter)
- Create a customized execution environment that includes VMware Ansible Collections
