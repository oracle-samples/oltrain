---
title: "Enable Oracle Ksplice"
date: 2021-09-09
draft: false
summary: "Learn to set up an Oracle Ksplice enhanced client through an online connection with the Unbreakable Linux Network (ULN)."
tags: ["ol","tutorial","ol-ksplice"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-ksplice-enable)

## Details

Oracle Ksplice provides a method of patching your Oracle Linux system that has the following advantages:

   - Critical security patches for Linux kernels, hypervisors, and critical userspace libraries are applied immediately.
   - Updates are non-intrusive because the process does not require reboots and system downtime.

Two modes are available for setting up an Oracle Ksplice client: the online mode and the offline mode. Moreover, you can set up either a standard client, where only the kernel is updated, or an enhanced client, which supports userspace and Xen and adds known exploit detection.

Some information sources refer to the Ksplice uptrack client. The uptrack client is a subset of the functionality of the enhanced client and only patches the kernel. In other words, this tutorial refers to the uptrack client when describing the standard client.

> **Note:** Oracle Ksplice is automatically installed and enabled on Oracle Linux instances running on Oracle Cloud Infrastructure (OCI). You do not need to register these instances with ULN to use Oracle Ksplice.

### Objectives

In this tutorial, you'll learn how to:

   - Set up an enhanced client through an online connection with the Unbreakable Linux Network (ULN)
   - Register with Unbreakable Linux Network (ULN) and install the necessary Oracle Ksplice packages.

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the internet
    - Obtain a Customer Support Identifier (CSI) by creating an account with ULN
