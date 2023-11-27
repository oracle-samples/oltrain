---
title: "Storage Management"
date: 2020-08-03
weight: 03
draft: false
description: "Storage Management"
summary: "When working with Oracle Linux, the environment you are accessing is not always physically accessible. In those cases, you need to know how to administer your environment remotely. Watch these short videos on how to establish secure connections to remote Oracle Linux 8 systems. With secure connections, all traffic transmitted over the wire is encrypted and protected from password sniffing attacks and other outside monitoring."
tags: ["partitions","fstab","nfs","btrfs","filesystems"]
slug: "stor-mgmt"
showRecent: false
showDate: false
showLikes: false
showViews: false
showEdit: false
showReadingTime: false
showAuthor: false
showDateUpdated : false
sharingLinks : false
cascade:
  showDate: false
  showAuthor: false
  invertPagination: true
aliases:
- /OL/stor_mgmt/stor_mgmt.html
series: ["Oracle Linux"]
series_order: 10
---

## Videos

{{< lead >}} Whether manually partitioning your primary disk, adding additional disks for storage, or creating shared storage, working with disks is a skill all Linux Administrators should know. These videos will get you started on using fdisk, formatting, filesystems, and disk encryption. {{< /lead >}}

### Disk Partitioning with fdisk on Oracle Linux

- {{< youtube 3edFvAXe4Hs >}}

### Using Ext2, Ext3 and Ext4 File Systems on Oracle Linux

- {{< youtube fCuxJkrXf2w >}}

### Mounting File Systems on Oracle Linux

- {{< youtube 2cHm9ohqZJo >}}

### Using fstab to Mount Devices on Oracle Linux

- {{< youtube zO9kbExt3uI >}}

### Using Swap Space on Oracle Linux

- {{< youtube rv6iXD8Iod0 >}}

### Configure an NFS Server on Oracle Linux

- {{< youtube fnVoVzB8Px0 >}}

### Mount an NFS Export on Oracle Linux

- {{< youtube YFeaOEgFrto >}}

### Automount NFS Shares on Oracle Linux

- {{< youtube Fzvb2LKJdok >}}

### Using the XFS File System on Oracle Linux

- {{< youtube OUW1cbR-WuA >}}

### Get Started with the Btrfs File System on Oracle Linux

- {{< youtube hu3xX3o3ciA >}}

### Btrfs Subvolumes and Snapshots on Oracle Linux

- {{< youtube xH305gNQvJ8 >}}

### Using Snapper to Automate Btrfs Snapshots on Oracle Linux

- {{< youtube U3Ur9x_gZSg >}}

### Introduction to GlusterFS on Oracle Linux

- {{< youtube N7BeDUOcKg4 >}}
  
### Logical Volume Management on Oracle Linux

- {{< youtube 2ebupdOpOn8 >}}

## Labs

{{< lead >}} Each hands-on lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment. {{< /lead >}}

### [Work with File Systems on Oracle Linux](https://luna.oracle.com/lab/bbfe7177-f27a-42f5-97cf-95b7027efa26)

Learn how to use fdisk, mkfs, mount, swapon, and parted when working with file systems.

In the following lab, you list the mounted file systems. In addition, you partition disk devices and mount file systems. Then, you add entries in the file system table to mount file systems on reboots, and increase swap space. Lastly, you remove partitions and additional swap space.

---

### [Configure Logical Volumes on Oracle Linux](https://luna.oracle.com/lab/545675ec-9c52-42a5-b823-a7efb1ed237c)

Learn how to use LVM utilities to create and work with logical volumes.

Logical Volume Management allows combining multiple individual hard drives or disk partitions into a single volume group (VG). That volume group can then be subdivided into logical volumes (LV) or used as a single large volume. Standard file systems, such as EXT4 or XFS, can be created on a logical volume.

This lab will work with the Oracle Linux Volume Manager utilities to create, mount and increase the capacity of logical volumes.

---

### [Create an NFS Server on Oracle Linux](https://luna.oracle.com/lab/3e7b391f-db29-405d-85bc-b70ad5753dd4)

Learn how to install and configure an NFS server, and mount NFS shares.  The following lab provides step-by-step procedures to install and configure an NFS Server and mount the NFS shares. This tutorial is targeted at users of Oracle Linux.  In this lab you create an encrypted XFS file system that is automatically unlocked at boot when on the same network as your key server. This tutorial is targeted at users of Oracle Linux 8 or later.

---

### [Use autofs on Oracle Linux](https://luna.oracle.com/lab/5847ea10-bead-4dda-be13-72b55551f6a2)

Learn to use autofs to mount NFS shares automatically.  The following lab provides step-by-step procedures to configure autofs to mount NFS shares. The benefit of autofs is the file system is mounted only when accessed. This tutorial is targeted at users of Oracle Linux.

---

### [Use Network-Bound Disk Encryption on Oracle Linux](https://luna.oracle.com/lab/e348bfed-8e08-4b12-8114-74e87eb12497)

Learn how to use Network-Bound Disk Encryption on Oracle Linux.  The following lab shows you how to configure an Oracle Linux system with disk encryption that is dependent on a network based key service.  In this lab you create an encrypted XFS file system that is automatically unlocked at boot when on the same network as your key server. This lab is targeted at users of Oracle Linux 8 or later.

---

### [Set up Gluster Storage on Oracle Linux](https://luna.oracle.com/lab/4de49ca0-6b00-4c69-95a7-a60a4b21ab78)

Learn how to set up Gluster Storage on Oracle Linux 8 or later.

---

### [Get Started With the Btrfs File System on Oracle Linux](https://luna.oracle.com/lab/03f1fb2b-d4ef-4d1e-8a12-793cb3e3ffd8)

Learn how to use the Btrfs file system on Oracle Linux, including btrfs commands to perform common administrative Btrfs tasks.

The Btrfs file system provides the capacity to handle pooling, snapshots, checksums, and multi-device spanning in existing Linux file systems. For an overview of the Btrfs file system and its features, see Oracle Linux 8: Managing Local File Systems .

This lab describes how to set up your Oracle Linux system to use the Btrfs file system. This lab is targeted at users of Oracle Linux 8 or later.

---

### [Create a Highly Available NFS Service with Gluster and Oracle Linux](https://luna.oracle.com/lab/2bf5d9a2-7afc-4286-97ef-386427e3ebea)

Learn how to install and configure a highly available NFS service on Oracle Linux using Corosync, Pacemaker, Gluster and Ganesha.

In this lab, we will create an NFS service hosted by three instances: ol-node01, ol-node02, and ol-node03. These instances will replicate a Gluster volume for data redundancy and use clustering tools for service redundancy.

A fourth instance named ol-client will mount this NFS service for demonstration and testing.

This lab is targeted at Oracle Linux 8 users, but the commands are also available on other Oracle Linux releases.

---

### [Configure RAID Logical Volumes on Oracle Linux](https://luna.oracle.com/lab/2edede28-75f0-4046-8567-4cfd1596f931)

Learn how to configure RAID Logical Volumes on Oracle Linux.

LVM RAID is a way to create a Logical Volume (LV) that uses multiple physical devices to improve performance or tolerate device failures. In LVM, the physical devices are Physical Volumes (PVs) in a single Volume Group (VG).

This lab will work with the Oracle Linux Volume Manager utilities to create a RAID logical volume and then address a disk failure.

---

### [Build a Software RAID Array on Oracle Linux](https://luna.oracle.com/lab/2c5aab94-cacb-4978-b0c9-aca5c953f6e4)

Learn how to build a RAID array using the Oracle Linux kernel multidisk driver.

A Redundant Array of Independent Disks or RAID device is a virtual device created from two or more real block devices. This functionality allows multiple devices (typically disk drives or partitions of a disk) to be combined into a single device to hold a single filesystem. Some RAID levels include redundancy, allowing the filesystem to survive some degree of device failure.

The Oracle Linux kernel uses the Multiple Device (MD) driver to support Linux software RAID and enable you to organize disk drives into RAID devices and implement different RAID levels.

For more information on these different RAID levels, see the Oracle documentation .

This lab will work with the MD utility (mdadm) to create a RAID1 device with a spare and then address a disk failure.

---

### [Reduce and Relocate Volume Groups on Oracle Linux](https://luna.oracle.com/lab/ee495d1a-4e00-4d77-9719-2f27591d1ecd)

Learn how to remove a physical volume from a volume group and then move the volume group to another server.

Logical Volume Management allows for removing unused physical volumes (PVs) and for the moving of an entire volume group (VGs). The removal of a PV shrinks the overall size of the VG.

This lab will work with the Oracle Linux Volume Manager utilities to shrink a volume group by removing a physical volume and then transferring the volume group to another system.

---

### [Use and Enable ACLs on Oracle Linux](https://luna.oracle.com/lab/7a272852-6042-47e3-b25f-eb681c733e66)

Learn how to use and enable ACLs on Oracle Linux.

Access Control Lists (ACLs) provide access control to directories and files. ACLs can set read, write, and execute permissions for the owner, group, and all other system users.

An ACL consists of a set of rules that specify how a specific user or group can access ACL enabled files and directories. A regular ACL entry specifies access information for a single file or directory. A default ACL entry is set on directories only, and specifies the default access information for any file within the directory that does not have an access ACL.

When setting a default ACL on a directory, its subdirectories inherit the same rights automatically. ACLs can be used with the btrfs, ext3, ext4, OCFS2, and XFS file systems, as well as mounted NFS file systems.

---

### [Encrypt Drives using LUKS on Oracle Linux](https://luna.oracle.com/lab/9c62956d-153b-4e93-84b0-0b2759f7e4bb)

Learn how to encrypt a device using LUKS on Oracle Linux.

Oracle Linux includes device mapper crypt (dm-crypt) and the Linux Unified Key Setup (LUKS) to handle encryption on block devices.

In this lab, we'll focus on the front-end tools to encrypt a device using LUKS, which utilizes the dm-crypt module from the device mapper support included with the Linux Kernel.

---

{{< figure src="/img/quiz1.png" alt="ol-stor-mgmt-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:CPXRPS0" target="_blank" >}}
Take the quiz
{{< /button >}}
