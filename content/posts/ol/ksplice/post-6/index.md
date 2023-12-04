---
title: "Use Oracle Ksplice"
date: 2021-09-20
draft: false
summary: "Learn how to perform various Ksplice related tasks on Oracle Linux."
tags: ["ol","lab","tutorial","ol-ksplice"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/7bf9e1e8-691e-42d4-823d-6a0fad49791c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-ksplice-use)

## Details

Oracle Ksplice provides a method of patching your Oracle Linux system that has the following advantages:

  - Critical security patches for Linux kernels, hypervisors and critical user space libraries are applied immediately.
  - Updates are non-intrusive because the process does not require reboots and system downtime.

### Objectives

This tutorial describes useful Oracle Ksplice commands for obtaining information related to updating systems with the latest packages from Unbreakable Linux Network (ULN).

### Prerequisites

- An Oracle Linux system that has been set up as an Oracle Ksplice client, either as a standard or an enhanced client. The system must also have access to the Internet.
- If the Ksplice client is configured in online mode, it must be registered with the [Unbreakable Linux Network](https://linux.oracle.com).

  Clients can operate either in online or offline mode. This tutorial assumes that you have a Ksplice client that is configured in online mode.

If your system is not yet configured as an Oracle Ksplice client, see [https://docs.oracle.com/en/learn/oracle-linux-ksplice-enable](https://docs.oracle.com/en/learn/oracle-linux-ksplice-enable).

> **Note:** Oracle Ksplice is automatically installed and enabled on Oracle Linux instances that are running on Oracle Cloud Infrastructure (OCI). You do not need to register these instances with ULN to be able to work with Ksplice.


