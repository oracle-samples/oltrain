---
title: "Use and Enable ACLs"
date: 2022-07-19
draft: false
summary: "Learn how to Use and Enable ACLs"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/7a272852-6042-47e3-b25f-eb681c733e66)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-acls)

## Details

Access Control Lists (ACLs) provide access control to directories and files. ACLs can set read, write, and execute permissions for the owner, group, and all other system users.

An ACL consists of a set of rules that specify how a specific user or group can access ACL-enabled files and directories. A regular ACL entry specifies access information for a single file or directory. A default ACL entry is set on directories only and specifies the default access information for any file within the directory that does not have an access ACL.

When setting a default ACL on a directory, its subdirectories inherit the same rights automatically. You can use ACLs with the `btrfs`, `ext3`, `ext4`, `OCFS2`, and `XFS` file systems, as well as mounted NFS file systems.

### Objectives

In this tutorial, you'll learn how to:

   - Check file system ACL support
   - Use `setfacl` and `getfacl` commands to add and display ACL rules

### Prerequisites

  - Minimum of one Oracle Linux system

  - Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - An additional block device
