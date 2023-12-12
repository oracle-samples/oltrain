---
title: "Get Started with the Btrfs File System"
date: 2021-11-01
draft: false
summary: "Learn how to get started with the Btrfs File System"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/03f1fb2b-d4ef-4d1e-8a12-793cb3e3ffd8)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/btrfs-ol8)

## Details

The Btrfs file system provides the capacity to handle pooling, snapshots, checksums, and multi-device spanning in existing Linux file systems. For an overview of the Btrfs file system and its features, see [Oracle Linux 8: Managing Local File Systems](https://docs.oracle.com/en/operating-systems/oracle-linux/8/fsadmin/btrfs-main.html#xd_co_f=NjUzNDIzODAtMTcwNy00YzFlLTgxMDItNTM2YjIwZjBkMmQ0~) .

This tutorial describes how to set up your Oracle Linux system to use the Btrfs file system. This tutorial is targeted at users of Oracle Linux 8 or later.

### Objectives

In this tutorial, you will learn how to:

- Create a Btrfs file system on Oracle Linux 8
- Run basic Btrfs commands to perform tasks such as:
  - Checking file system usage
  - Extend the size of the file system
  - Recover a missing device
- Test and see how the file system works

### Prerequisites

The tutorial uses the following system:

- An Oracle Linux 8 system with the following configurations:
  - has multiple storage devices installed
  - runs the UEKR6 kernel
