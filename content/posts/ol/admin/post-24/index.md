---
title: "Use SELinux"
date: 2022-04-18
draft: false
summary: "Learn how to run SELinux on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/89a09fdd-47c2-4755-b98e-35863bdf7bc0)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-selinux)

## Details

SELinux, or Security-Enhanced Linux, is a set of kernel modifications and user-space tools designed to protect the Linux Operating System. SELinux is a Linux kernel security module that uses a mechanism called mandatory access controls (MAC) to provide another layer of system security, precise access control, system-wide admin-defined policies, and improved mitigation for privilege escalation attacks as defined by the system administrator.

This tutorial guides you through using these user-space tools to help keep your system running in enforcing mode.

### Objectives

In this tutorial, you will learn how to:

   - Check SELinux mode and status
   - Understand SELinux security labels
   - Work with SELinux network services
   - Use SELinux users
   - Change SELinux booleans
   - Evaluate SELinux file contexts

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
