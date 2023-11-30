---
title: "Automate Setup of Oracle Linux"
date: 2021-10-15
draft: false
summary: "Learn to use Oracle Linux Automation Engine to perform the initial configuration of an Oracle Linux instance."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/56b90194-88ab-421e-bc93-2ac708dce6ba)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-setup-ol8)

## Details

These guides provide a playbook for automating the initial setup of Oracle Linux using the configuration management tool Oracle Linux Automation Engine.

### Objectives

In this lab, you'll learn about writing and running a playbook that:

   - Creates a user
   - Adds the user to the `sudo` group
   - Copies a local SSH public key to the user's `authorized_keys` file

### What Do You Need?

  - A minimum of two Oracle Linux systems with the following configuration:

      - a non-root user with `sudo` permissions
      - ssh keypair for the non-root user
      - the ability to ssh from one host (control-node) to the other (host) using passwordless ssh login

