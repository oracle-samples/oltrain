---
title: "Create an NFS Server"
date: 2021-03-23
draft: false
summary: "Learn how to install and configure an NFS server, mount NFS shares, and use the autofs utility."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/3e7b391f-db29-405d-85bc-b70ad5753dd4)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/ol-nfs)

## Details

What is NFS? Network File System (NFS) is a protocol for a distributed file system that allows users to read and write files over the network and interact with them as if they are mounted locally. Developed by Sun Microsystems in 1984, NFS continues to be a popular way to consolidate resources and then share them on the network. Currently, Oracle Linux supports NFS version 3 (NFSv3) and NFS version 4 (NFSv4) and will default to NFSv4 when mounting shares if the server supports it.

### Objectives

In this tutorial, you will learn how to:

  - Install the NFS utility package
  - Configure an NFS server
  - Mount NFS shares
  - Configure the autofs utility

### Prerequisites

- Minimum of two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Key-based SSH, also known as password-less SSH, between the hosts
    - Access to the Internet
