---
title: "Configure RAID Logical Volumes"
date: 2022-05-23
draft: false
summary: "Learn how to configure RAID Logical Volumes"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/2edede28-75f0-4046-8567-4cfd1596f931)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-lvmraid)

## Details

LVM RAID is a way to create a Logical Volume (LV) that uses multiple physical devices to improve performance or tolerate device failures. In LVM, the physical devices are Physical Volumes (PVs) in a single Volume Group (VG).

This tutorial will work with the Oracle Linux Volume Manager utilities to create a RAID logical volume and then address a disk failure.

### Objectives

In this tutorial, you will learn how to:

- Create a RAID logical volume
- Resize a RAID logical volume
- Recover a failed RAID device

### Prerequisites

The tutorial uses the following system:

- Any Oracle Linux 8 system with the following configurations:
  - a non-root user with sudo permissions
  - additional block volumes for use with LVM
