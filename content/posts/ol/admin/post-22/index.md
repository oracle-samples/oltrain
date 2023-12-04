---
title: "Upgrade with LEAPP"
date: 2022-03-31
draft: false
summary: "Learn how to upgrade current release Oracle Linux 7 to current release Oracle Linux 8 using Leapp."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/908d0e5b-4444-400a-87a7-2a9ec8c27550)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-linux-leapp)

## Details

The Leapp utility is a framework for updating and upgrading operating systems as well as applications. The utility's component packages enable the creation of different workflows into profiles for updating software.

Leapp operations consist of two phases:

- **Preupgrade -** a process that examines many aspects of the system and runs checks to determine if the OS software can be upgraded.
- **Upgrade -** updates the system based on configuration files that map packages between previous and current versions of the software.

Leapp can be used to upgrade Oracle Linux 7 Oracle Cloud Infrastructure instances, as well as Oracle Linux 7 on premise systems.

These guides walk you through upgrading a current release Oracle Linux 7 Oracle Cloud Infrastructure instance to Oracle Linux 8.

Leapp is not supported for any other operating systems or versions.

> **Note:** Before using Leapp in a production environment it is recommended to become familiar with the Leapp upgrade process in a test environment. This allows you to better understand the process, its reports, and test for any security or compatibility issues that might be encountered.

### Objectives

In this lab, you'll learn to:

   - Prepare an Oracle Linux 7 system and use Leapp to upgrade to Oracle Linux 8
   - Check and modify prerequisite settings to the system to support the Leapp upgrade
   - Perform a preupgrade check to inspect and create reports on the system configuration and items to be addressed before upgrading
   - Perform an upgrade of the system to Oracle Linux 8 using the Leapp utility

### Prerequisites

  - An Oracle Cloud Infrastructure instance running the current release Oracle Linux 7

