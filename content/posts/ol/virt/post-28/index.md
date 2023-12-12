---
title: "Mount a NFS Share"
date: 2022-09-22
draft: false
summary: "Learn how to use an NFS share as a volume for remote and persistent storage within a Podman container."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/556e1401-568f-447e-8c0b-c94a86b1114f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-volume-nfs)

## Details

A Network File System or NFS is a distributed file system protocol originally developed by Sun Microsystems in 1984. NFS allows a user on a client computer to access files over the network, similar to how they access local storage.

When working with Podman containers, the need may arise to access files on an NFS share, which you accomplish using a Podman volume. Volumes are the preferred means to persist data generated and used by the containers. Podman completely manages volumes and differs from bind mounts as they are independent of the host machine's directory structure and OS.

These guides will show how to use Podman volumes to mount and access a remote NFS share.

### Objectives

  - Create an NFS-backed Podman volume
  - Read and write to the Podman volume

### What Do You Need?

  - A client system with Oracle Linux installed
  - An up-and-running NFS server with a shared data directory

