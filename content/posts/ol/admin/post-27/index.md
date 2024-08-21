---
title: "Disable Kernel Module"
date: 2023-05-03
draft: false
summary: "Learn how to disable a kernel module and prevent it from loading at boot time."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/00aafe17-39b9-43e0-8b53-087b84003c15)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-kernel-module-disable)

## Details

As a Linux administrator, there will come a time when you want to disable kernel modules for hardware that might be causing a problem on a system, or it gets flagged for a vulnerability.

### Objectives

In this tutorial, you will learn how to:

  - Disable a module using modprobe
  - Add the module to the kernel module deny list
  - Create a backup of the existing initramfs
  - Rebuild the initramfs by using dracut to exclude the module

> **Note:** Disabling modules can have unintended consequences and prevent a system from booting properly or being fully functional after boot. Therefore, we'll demonstrate creating a backup ramdisk image as best practice to ensure you can recover if a change prevents booting the operating system.

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
