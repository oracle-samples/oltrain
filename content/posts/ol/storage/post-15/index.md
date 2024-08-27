---
title: "Work with File Systems"
date: 2021-07-14
draft: false
summary: "Learn how to create and mount file systems on Oracle Linux."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/bbfe7177-f27a-42f5-97cf-95b7027efa26)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-file-systems)

## Details

Partitioning a disk is one of the first tasks when creating a file system. It divides the space on the disk but does not allow the operating system to store files on it. The ability to store files on a disk occurs when you format it with a file system. Oracle Linux supports many file systems, but we will focus on ext4 and xfs.

### Objectives

In this tutorial, you'll learn how to:

   - Display the current partition table
   - List mounted file systems
   - Partition disk devices
   - Create and mount file systems on partitions
   - Modify the file system table to mount the file systems on reboots
   - Increase the amount of swap space
   - Remove partitions and additional swap space

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - Two or more block devices attached to the system  
