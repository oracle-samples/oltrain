---
title: "Create a Highly Available NFS Service with Gluster"
date: 2022-05-09
draft: true
summary: "Learn how to create a highly available NFS Service with Gluster"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/2bf5d9a2-7afc-4286-97ef-386427e3ebea)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-ha-nfs)

## Details

In this lab, we will create an NFS service hosted by three instances: ol-node01, ol-node02, and ol-node03. These instances will replicate a Gluster volume for data redundancy and use clustering tools for service redundancy.

A fourth instance named ol-client will mount this NFS service for demonstration and testing.

This tutorial is targeted at Oracle Linux 8 users, but the commands are also available on other Oracle Linux releases.

## Components

- **Corosync** provides clustering infrastructure to manage which nodes are involved, their communication, and quorum.
- **Pacemaker** manages cluster resources and rules of their behavior.
- **Gluster** is a scalable and distributed filesystem.
- **Ganesha** is an NFS server that can use many different backing filesystem types, including Gluster.

### Objectives

In this tutorial, you will learn how to:

- Create a Gluster volume
- Configure Ganesha
- Create a Cluster
- Create Cluster services

### Prerequisites

The tutorial uses the following system:

- Four Oracle Linux 8 instances installed with the following configuration:
  - a non-root user with sudo permissions
  - ssh keypair for the non-root user
  - ability to ssh from one host (ol-node01) to the others (ol-node02,ol-node03) using passwordless ssh login
  - additional block volume for use with gluster
