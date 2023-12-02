---
title: "Use OCFS Tools"
date: 2022-03-03
draft: false
summary: "Learn how to configure an Oracle Cluster File System (OCFS2) on Oracle Cloud Infrastructure."
tags: ["oloci","lab","tutorial","oloci-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a7e62a2a-10d0-4b11-a317-bf559c99b148)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocfs2_cluster_linux_8)

## Details

OCFS2 is a general-purpose clustered file system used in clustered environments to increase storage performance and availability. In Oracle Cloud Infrastructure, you can deploy OCFS2 clustered file systems through **Read/Write - shareable** block storage attached to an instance.

> **Note:** For optimal OCFS2 file system performance, reduce the number of files with the OCFS2 filesystem. Applications such as Oracle e-Business Suite (EBS) or Oracle WebCenter Content (WCC) should leverage a separate NFS file system for directories containing large amounts of temporary files. During runtime, system administrators should actively archive, purge, remove, delete, and move any non-current files to one or more separate subdirectories or filesystems while regularly monitoring the OCFS2 filesystem file/inode usage.

These guides provide instructions on using `ocfs2-tools` to deploy and test a two node Oracle Cluster File System version 2 (OCFS2) on Oracle Cloud Infrastructure.

### Objectives

  - Prepare for an OCFS2 configuration
    - Configure security list
    - Create and attach a block volume
  - Install or upgrade the software required for OCFS2
  - Configure the cluster layout
  - Configure and start the O2CB cluster stack service
  - Create an OCFS2 volume
  - Mount an OCFS2 volume

### Prerequisites

Two Oracle Linux systems with the following configuration:

- a non-root user with sudo permissions
- Oracle Linux 8 or later and the latest UEK kernel
- additional block volumes for use with OCFS2

