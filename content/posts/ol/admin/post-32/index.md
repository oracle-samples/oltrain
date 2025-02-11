---
title: "Explore System Configuration Files and Kernel Tunables"
date: 2022-02-22
draft: false
summary: "Learn to use the sysctl command and explore the /proc, /sys and /etc/sysconfig file systems."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/aa8f2377-7967-4e45-bf32-bdc8054d5c76)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-sysctl)

## Details

Oracle Linux provides many ways to customize your system's configuration. A system's configuration includes arguments for various services in config files found in the `/etc/sysconfig` directory and runtime kernel tuning parameters under the `/proc/sys` file system. Whether you set the configuration changes as transient or persistent, each parameter and value impacts how your system runs and behaves.

### Objectives

In this tutorial, you'll learn to:

- View system configuration files
- Modify kernel settings
- View hardware device and device driver attributes

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account with sudo access
  - Access to the Internet
