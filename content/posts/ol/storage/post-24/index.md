---
title: "Reduce and Relocate Volume Groups"
date: 2022-06-13
draft: false
summary: "Learn how to Reduce and Relocate Volume Groups"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/ee495d1a-4e00-4d77-9719-2f27591d1ecd)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-move-lvm)

## Details

Logical Volume Management allows for removing unused physical volumes (PVs) and moving an entire volume group (VGs). The removal of a PV shrinks the overall size of the VG.

This tutorial will work with the Oracle Linux Volume Manager utilities to shrink a volume group by removing a physical volume and then transferring the volume group to another system.

### Objectives

In this tutorial, you will learn how to:

   - Move a logical volume
   - Shrink a volume group
   - Transfer a volume group to another system

### Prerequisites

- Minimum of two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
   - A non-root user account with sudo access
   - Additional block volumes for use with LVM
