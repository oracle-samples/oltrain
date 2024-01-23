---
title: "Enable the EPEL Repository"
date: 2024-01-23
draft: false
summary: "Learn to use Oracle Linux Automation Engine to add the EPEL Repository to an Oracle Linux instance."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/332e5b39-b951-41ff-b322-b62ccb8d6988)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-add-repo)

## Details

This tutorial provides a playbook for automating the addition of a software repository to an Oracle Linux instance using the configuration management tool Oracle Linux Automation Engine.

### Objectives

In this lab, you'll learn to:

   - Add the EPEL repository to an Oracle Linux install
   - Use the repository to install a package

### Prerequisites

  - Install an Oracle Linux system with the following configuration:
      - a non-root user with `sudo` permissions
      - ssh keypair for the non-root user
      - the ability to ssh from one host (control-node) to the other (host) using passwordless ssh login
