---
title: "OCI iSCSI Utility"
date: 2022-01-12
draft: false
summary: "Learn how to use the OCI iSCSI Utility to manage iSCSI block volumes on Oracle Cloud Infrastructure."
tags: ["oloci","tutorial","oloci-storage"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oci-sys-admin)

## Details

In these guides, you learn how to enable and configure the OCI Utilities, and then run `oci-iscsi-config` to manage iSCSI block volumes on an Oracle Cloud Infrastructure instance.

### Background

Before the OCI Utilities package was available, you had to use the iSCSI administration commands, through the cloud web console, to manually attach and detach the block devices to an instance.

With the `oci-iscsi-config` command and the `oci-utils` daemon, you can easily create and manage volume attachments on the instance and in the cloud.

When the `oci-utils` daemon runs, it automatically looks for iSCSI block volumes available in the cloud compartment and attached through the web console.

It also supports the creation and removal of devices in the cloud resources, as well as the attachment of those devices to and from the Linux instance.

### Objectives

- Install required software
- Setup Oracle Cloud Infrastructure config file
- Explore `oci-iscsi-config` command usage
- Create block volumes
- Attach block volumes
- Detach block volumes on an instance
- Destroy block volumes on an instance

### What Do You Need?

- A fully patched Oracle Linux system
