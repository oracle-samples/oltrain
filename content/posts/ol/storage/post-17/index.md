---
title: "Use autofs"
date: 2021-03-28
draft: true
summary: "Learn how to autofs to mount NFS shares automatically."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5847ea10-bead-4dda-be13-72b55551f6a2)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/autofs_linux8)

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
