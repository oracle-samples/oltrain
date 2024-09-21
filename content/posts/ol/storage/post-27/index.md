---
title: "Configure Logical Volumes"
date: 2022-05-23
draft: false
summary: "Learn how to use LVM utilities to create and work with logical volumes."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/545675ec-9c52-42a5-b823-a7efb1ed237c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-lvm)

## Details

Logical Volume Management allows combining multiple individual hard drives or disk partitions into a single volume group (VG). That volume group can then be subdivided into logical volumes (LV) or used as a single large volume. Standard file systems, such as EXT4 or XFS, can be created on a logical volume.

This tutorial will work with the Oracle Linux Volume Manager utilities to create, mount, and increase the capacity of logical volumes.

### Objectives

In this tutorial, you will learn to:

  - Create a logical volume
  - Increase the capacity of a logical volume

### Prerequisites

  - Minimum of one Oracle Linux system

  - Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - An additional block device
