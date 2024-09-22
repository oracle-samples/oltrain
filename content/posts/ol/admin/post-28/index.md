---
title: "ReaR Backups"
date: 2023-06-02
draft: false
summary: "Learn how to peform a backup of Oracle Linux using the Relax-and-Recover disaster recovery solution."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/30023183-ca96-48dc-8497-af04ca1eada4)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-backup-rear)

## Details

Relax-and-Recover (ReaR) was born in 2006 by Gratien D'haese and Schlomo Schapiro as part of a complete rewrite of an earlier Linux Disaster Recovery project mkCDrec. ReaR is an Open Source bare metal disaster recovery solution that Oracle Linux (OL) provides natively. It produces a bootable image that can recreate the system's original storage layout and restore from the backup.

ReaR is directly available from the Application Streams repository in Oracle Linux 8 or later and is simple to deploy and configure.

This tutorial guides users on installing and configuring ReaR to backup and restore Oracle Linux using NFS storage.

### Objectives

In this tutorial, you'll learn to:

- Install the ReaR package
- Configure ReaR to exclude specific filesystems, mount points, and Logical Volumes that are not needed
- Perform a ReaR backup using NFS storage as a backup repository
- Verify the ReaR client backup on the NFS storage
- Perform a ReaR recovery

### Prerequisites

- Minimum of three Oracle Linux systems

 - An Oracle Linux system as the ReaR client
 - An NFS server as the backup storage location
 - Another system for the recovery

> We'll leverage KVM in this tutorial to create virtual machines for the required systems.
