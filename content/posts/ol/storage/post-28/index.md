---
title: "Use Btrfs for Root Level Snapshots"
date: 2024-08-12
draft: false
summary: "Learn to use a root Btrfs file system to get system-level snapshots using Snapper on Oracle Linux."
tags: ["ol", "tutorial", "ol-storage"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-btrfs-root-snapshots)

## Details

As with any operating system, you must apply patches to keep it current and secure. But what if something goes wrong with an update or system files get deleted? Having a process in place to perform a restore is vital.

While you may be familiar with traditional backup and restore, you gain additional options when using [Btrfs as your root file system](https://docs.oracle.com/en/operating-systems/oracle-linux/9/install/install-InstallingaSystemWithaBtrfsrootFileSystem.html#install-btrfs-filesystem). Using Btrfs requires booting into Oracle's Unbreakable Enterprise Kernel (UEK) release and provides the option to use Snapper or Btrfs's snapshot send and receive feature for remote incremental backups.

This tutorial describes how to perform a backup and restore using Btrfs snapshot and Snapper to recover from a system failure.

### Objectives

In this tutorial, you will learn how to:

   - Verify you're running a Btrfs root file system
   - Create a snapshot
   - Snapper
   - Restore

### Prerequisites

- Minimum of a single Oracle Linux system running the UEK kernel

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - Btrfs root file system
