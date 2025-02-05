---
title: "Use Grubby"
date: 2023-08-02
draft: false
summary: "Learn to use grubby to manage the boot kernel in Oracle Linux."
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/67f106f2-8c50-442c-b24f-108b806be84f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-grubby)

## Details

*Grubby** is a flexible and powerful command-line tool that provides users with an easy way to modify the bootloader configuration used by Oracle Linux without users having to manually edit the GRUB (GRand Unified Bootloader) or GRUB2 configuration files directly. In most cases, changing the default kernel is unnecessary because Oracle Linux defaults to a configuration and behavior to use and boot the most recent kernel version first. **Grubby** is also scriptable, making managing your system's default kernel requirements easier. Reasons why you should consider using **grubby** include:

- It has a simple command-line structure that makes managing bootloader settings much easier.
- It provides an easy way to list and manage multiple kernels, simplifying updating kernel parameters or changing the default kernel.
- It works with both UEFI and BIOS-based systems.
- It removes the risk associated with manual editing of bootloader files directly.

### Objectives

In this tutorial, you'll learn how to:

- Determine the currently loaded kernel
- Determine the default kernel
- Determine which kernel versions are available on the system
- Use **grubby** to manage kernels

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account with sudo access
  - Access to the Internet
