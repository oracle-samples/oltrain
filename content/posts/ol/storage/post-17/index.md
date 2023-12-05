---
title: "Use autofs"
date: 2021-03-28
draft: false
summary: "Learn how to autofs to mount NFS shares automatically."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/3e7b391f-db29-405d-85bc-b70ad5753dd4)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/create_nfs_linux)

## Details

The following tutorial provides step-by-step procedures to configure autofs to mount NFS shares. The benefit of autofs is the file system is mounted only when accessed. This tutorial is targeted at users of Oracle Linux.

### Objectives

In this tutorial, you will learn how to:

- Install nfs-utils
- Configure an NFS server
- Mount NFS shares

### Prerequisites

The tutorial uses the following system:

- A client system with Oracle Linux installed.
- An NFS server up and running with a shared data directory at `/nfs-share`.
