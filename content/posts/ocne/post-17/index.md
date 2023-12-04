---
title: "Provision PersistentVolumes Using File Storage Service on Oracle Cloud Native Environment"
date: 2023-03-23
draft: false
summary: "This tutorial will focus on OCI File System service to provide nfs-style cloud storage."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Provision PersistentVolumes Using File Storage Service on Oracle Cloud Native Environment](https://luna.oracle.com/lab/5d95fdca-c690-4ebf-8ac0-315ac095ac59)

:spiral_notepad: [Provision PersistentVolumes Using File Storage Service on Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-pv-fss)

## Details

Oracle Cloud Native Environment ships with the ability to install the Oracle Cloud Infrastructure (OCI) Cloud Controller Manager (CCM). The CCM is OCI's implementation of the Kubernetes control plane component that links your Kubernetes cluster to OCI.

The OCI CCM project implements a Container Storage Interface (CSI) plugin for Kubernetes clusters that implements both OCI Block Volume Storage and OCI File Storage Service to store persistent data.

This tutorial will focus on OCI File System service to provide nfs-style cloud storage.

> **Note:** Please note that Oracle Cloud Native Environment upgrades are incremental and not cumulative.  This is due to a limitation from both the Kubernetes and Istio modules which require incremental upgrades.

### Objectives

In this tutorial, you will learn how to:

- Create an OCI File System service
- Create a PersistentVolume based on the OCI File System service
- Claim the PersistentVolume
- Use the PersistentVolume

### Prerequisites

- Install Oracle Cloud Native Environment with the CCM module installed
- An Oracle Cloud Infrastructure (OCI) account
- A user in the OCI account with permission to work with resources in a compartment
- Access to that accounts credentials and OCID information
- A Virtual Cloud Network (VCN) with the following security rules to allow network traffic to and from the mount target:
  - Stateful ingress to TCP ports 111, 2048, 2049, and 2050, and UDP ports 111 and 2048.
  - Stateful egress for TCP source ports 111, 2048, 2049, and 2050, and UDP source port 111.
