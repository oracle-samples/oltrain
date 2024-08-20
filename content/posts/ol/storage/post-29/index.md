---
title: "Use Btrfs Send and Receive"
date: 2024-08-20
draft: false
summary: "Learn how to use the Btrfs send and receive features to remotely back up a subvolume over SSH."
tags: ["ol", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/b8f5ee68-75fe-4790-a3ab-c7be5f5461fd)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-btrfs-send)

## Details

Having a backup is essential to avoid losing data. Using Btrfs and its send and receive features, we can configure secure sender and receiver systems to securely and efficiently remote backup a subvolume over SSH. Then, set up Systemd timers to perform regular, timely backups.

Note that only the changes made on the sender system are copied to the receiver system, reducing the backup facility's overhead. Since the systems use Btrfs snapshots, the disk usage for incremental backups is restricted only to the size of the changes.

### Objectives

In this tutorial, you will learn how to:

  - Configure SSH to facilitate secure network-based backup
  - Create a Btrfs receiver script on the receiver system
  - Create a Btrfs snapshot on the sender system
  - Send the Btrfs snapshot to the receiver system
  - Create an incremental backup snapshot
  - Create an incremental backup script
  - Configure a Systemd service and timer unit for regular incremental backups

### Prerequisites

- Minimum of two Oracle Linux systems running the UEK kernel

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - A block device attached to each system and formatted with Btrfs
    - Key-based SSH, also known as password-less SSH, between the hosts
