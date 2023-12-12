---
title: "Disable Kernel Module"
date: 2023-05-03
draft: false
summary: "Learn how to disable the bluetooth kernel module and to prevent it loading at boot time on Oracle Linux 8 and Oracle Linux 9 systems."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/00aafe17-39b9-43e0-8b53-087b84003c15)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-kernel-module-disable)

## Details

In this lab you unload a kernel module on an Oracle Linux instance and configure the system to prevent the module from loading at boot time. You can use this knowledge to disable kernel modules for hardware that might be causing a problem on a system or that may be flagged for a vulnerability.

### Objectives

These guides show how to disable the btrfs Linux kernel module on Oracle Linux and to prevent it from loading at boot time. The btrfs module is used for demonstration purposes but you could use the same procedure to disable any other Linux kernel module on a system. The main steps are outlined below:

  - Disable the module using modprobe
  - Add the module to the kernel module deny list
  - Create a backup of the existing initramfs
  - Rebuild the initramfs by using dracut to exclude the module

> **Note:** Disabling modules can have unintended consequences and can prevent a system from booting properly or from being fully functional after boot. In this tutorial we demonstrate creating a backup ramdisk image as best practice to make sure that you are able to recover in the event that a change prevents boot.

### What Do You Need?

  - A client system with Oracle Linux 8 or Oracle Linux 9 installed


