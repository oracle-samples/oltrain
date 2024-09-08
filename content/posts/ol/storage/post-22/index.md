---
title: "Build a Software RAID Array"
date: 2022-06-06
draft: false
summary: "Learn how to build a software RAID array"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/2c5aab94-cacb-4978-b0c9-aca5c953f6e4)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-mdadm)

## Details

A Redundant Array of Independent Disks or RAID device is a virtual device created from two or more real block devices. This functionality allows multiple devices (typically disk drives or partitions of a disk) to be combined into a single device to hold a single filesystem. Some RAID levels include redundancy, allowing the filesystem to survive some degree of device failure.

The Oracle Linux kernel uses the Multiple Device (MD) driver to support Linux software RAID. This driver enables you to organize disk drives into RAID devices and implement different RAID levels.

For more information on these different RAID levels, see the [Oracle documentation](https://docs.oracle.com/en/operating-systems/oracle-linux/8/stordev/stordev-WorkingWithSoftwareRAID.html#about-raid).

This tutorial will work with the MD utility (`mdadm`) to create a RAID1 device with a spare and then address a disk failure.

### Objectives

In this tutorial, you will learn how to:

   - Create a RAID1 device with a spare
   - Recover a failed RAID1 device

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - Two or more block devices attached to the system 
