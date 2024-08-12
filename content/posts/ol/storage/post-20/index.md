---
title: "Get Started with the Btrfs File System"
date: 2021-11-01
draft: false
summary: "Learn to create, extend, and recover a Btrfs file system on Oracle Linux."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/03f1fb2b-d4ef-4d1e-8a12-793cb3e3ffd8)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-btrfs)

## Details

The Btrfs file system provides the capacity to handle pooling, snapshots, checksums, and multi-device spanning in existing Linux file systems. For an overview of the Btrfs file system and its features, see [Oracle Linux: Managing Local File Systems](https://docs.oracle.com/en/operating-systems/oracle-linux/9/fsadmin/btrfs-main.html).

This tutorial describes setting up a directory on external storage on your Oracle Linux system to use the Btrfs file system.

### Objectives

In this tutorial, you will learn how to:

- Create a Btrfs file system
- Run basic Btrfs commands to perform tasks such as:
  - Checking file system usage
  - Extend the size of the file system
  - Recover a missing device
- Test and see how the file system works

### Prerequisites
- Minimum of a single Oracle Linux system running the UEK kernel

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet

