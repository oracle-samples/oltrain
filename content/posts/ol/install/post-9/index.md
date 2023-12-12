---
title: "Manage the Boot Kernel"
date: 2023-08-02
draft: false
summary: "Learn about the tools to use when managing the boot kernel on Oracle Linux."
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/67f106f2-8c50-442c-b24f-108b806be84f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-kernels)

## Details

These guides describe how to set the default kernel of an Oracle Linux system from the command line. This tutorial is targeted at Oracle Linux 8 users, but the commands are also available on other Oracle Linux releases.

### Background

By default, Oracle Linux systems are configured to boot the most recent kernel version first. In most cases, changing the default kernel is unnecessary.

In previous releases, setting the default kernel was performed by configuring the GRUB boot loader or by using other alternative commands. Now, however, you should preferrably use the **grubby** command to control and manage all of your boot requirements. This tool offers the benefit of being scriptable and can abstract bootloader configuration from the user.

### Objectives

In this lab, you'll learn how to:
-  determine the current loaded kernel
-  determine the default kernel
-  determine which kernel versions are available on the system
-  use **grubby** to manage kernels

### What Do You Need?

-   Any Oracle Linux system that has the `grubby` package installed

