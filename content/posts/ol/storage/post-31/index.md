---
title: "iSCSI Targets and Initiators"
date: 2025-03-25
draft: false
summary: "Learn to configure an iSCSI target on Oracle Linux to share block storage devices with another Oracle Linux instance using an iSCSI initiator."
tags: ["ol","lab","tutorial","ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/f85faa38-5476-41a0-951e-56dd86a8ba78)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-iscsi)

## Details

Oracle Linux uses the Linux-IO Target (LIO) to provide the block-storage SCSI target for FCoE, iSCSI, and Mellanox InfiniBand (iSER and SRP). For iSCSI (Internet Small Computer System Interface), an iSCSI target is a server, storage array, or device that hosts storage resources and provides them as SCSI block devices (LUNs) accessible over an IP network to iSCSI initiators.

An iSCSI initiator is a client device that uses the iSCSI protocol to send SCSI commands to an iSCSI target over an IP network, essentially acting as a client in a storage network.

### Objectives

In this tutorial, you'll learn how to:

- Configure an iSCSI target
- Configure an iSCSI Initiator

### Prerequisites

- Two Oracle Linux systems running the UEK kernel

- Each system should have Oracle Linux installed and configured with:
  - a non-root user with sudo permissions

- Attach two 50GB block volumes to one instance as read-write for use as iSCSI block devices

- OCI Ingress Rules allowing TCP and UDP traffic on port 3260. Security lists control the traffic in and out of the various subnets associated with the VCN.
