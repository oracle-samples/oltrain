---
title: "Upgrade with Leapp"
date: 2022-03-31
draft: false
summary: "Learn to upgrade the latest Oracle Linux 7 release to Oracle 8 and then to Oracle Linux 9 using the Leapp utility."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/908d0e5b-4444-400a-87a7-2a9ec8c27550)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-leapp)

## Details

The Leapp utility is a framework for updating and upgrading operating systems and applications. The utility's component packages enable the creation of different workflows into profiles for updating software.

Leapp operations consist of two phases:  

- **Preupgrade -** A process that examines many aspects of the system and runs checks to determine if the OS software can be upgraded.
- **Upgrade -** Updates the system based on configuration files that map packages between previous and current versions of the software.  

Leapp can be used to upgrade Oracle Linux Oracle Cloud Infrastructure instances, as well as Oracle Linux on-premise systems.  

This tutorial functions in two parts:

   1. It guides you through upgrading an Oracle Linux 7 instance to Oracle Linux 8.  
   1. It guides you through upgrading the same system from Oracle Linux 8 to Oracle Linux 9.

> **Note:** Before using Leapp in a production environment it is recommended to become familiar with the Leapp upgrade process in a test environment. This allows you to better understand the process, and its reports, and test for any security or compatibility and pre and post-upgrade issues that might be encountered.  
>
> The Leapp utility is used to upgrade the Operating System (OS) only, for example, from the current Oracle Linux 7 release to the current Oracle Linux 8, or the current Oracle Linux 8 to the current Oracle Linux 9. The procedures in this tutorial do not apply to and are unsupported on any other OS or versions.

### Objectives

In this tutorial, you'll learn to:  

- Prepare an Oracle Linux 7 system to use Leapp to upgrade to Oracle Linux 8, then prepare the same system to upgrade to Oracle Linux 9
- Check and modify prerequisite settings to the system to support the Leapp upgrade
- Perform a preupgrade check to inspect and create reports on the system configuration and items to be addressed before upgrading
- Use the Leapp utility to perform an upgrade of the system to Oracle Linux 8 and then perform another upgrade of the same system to Oracle Linux 9

### Prerequisites  

- An Oracle Linux instance running the latest release of Oracle Linux 7
