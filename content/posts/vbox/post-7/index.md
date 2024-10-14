---
title: "Use VirtualBox on Oracle Linux"
date: 2024-10-14
draft: false
summary: "Learn to create virtual machines and run Oracle VirtualBox on Oracle Linux."
tags: ["vbox","lab","tutorial","vbox7-1"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/922eabed-e47c-4934-a4a5-dbacc02f4f3b)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/vbox-oci)

## Details

Oracle VirtualBox is a cross-platform virtualization product that enables you to run multiple operating systems on your macOS, Windows, Linux, or Oracle Solaris systems. While providing the ability to run multiple virtual machines on a host system, VirtualBox also allows managing resources in Oracle Cloud Infrastructure.

You can read more detailed information about Oracle VirtualBox at this documentation link: [Oracle VirtualBox Documentation](https://docs.oracle.com/en/virtualization/virtualbox/index.html)

### Objectives

In this tutorial, you will learn to:

- Install Oracle VirtualBox on Oracle Linux
- Install the VirtualBox Extension Pack
- Use VirtualBox to create a new Oracle Linux virtual machine
- Install VirtualBox Guest Additions to a Virtual Machine

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - A graphical desktop
  - A VNC (Virtual Network Computing) server if running a headless/remote system

> If installing on an Oracle Cloud Infrastructure (OCI) instance, you'll need to use an Intel CPU shape such as *VM.Standard3.Flex*.
