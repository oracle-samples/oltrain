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

SELinux is a set of kernel mods and user-space tools that provide another layer of system security, precise access control, system-wide admin-defined policies, and improved mitigation for privilege escalation attacks.

These guides walk you through using these user-space tools to help keep your system running in enforcing mode.

### Objectives

In this lab, you'll learn to:

   - Check SELinux mode and status
   - Understand SELinux security labels
   - Work with SELinux network services
   - Use SELinux users
   - Change SELinux booleans
   - Evaluate SELinux file contexts

### Prerequisites

   - A system with Oracle Linux 8 installed with the following configuration:
      - a non-root user with `sudo` permissions


