---
title: "Use Network-Bound Disk Encryption"
date: 2021-06-21
draft: false
summary: "Learn how to use Network-Bound Disk Encryption."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/e348bfed-8e08-4b12-8114-74e87eb12497)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/nbde-oracle-linux)

## Details

The following tutorial shows you how to configure an Oracle Linux system with disk encryption that is dependent on a network based key service.

### Objectives

In this tutorial, you will learn how to:

- Create an encrypted XFS file system that is automatically unlocked at boot when on the same network as your key server 
- This tutorial is targeted at users of Oracle Linux 8 or later.

### Prerequisites

The tutorial uses the following system:

- Two systems with Oracle Linux 8 installed.
- A disk or block device attached to one system to use for encrypted storage
