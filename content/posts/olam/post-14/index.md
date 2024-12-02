---
title: "Run Oracle Linux Tasks"
date: 2024-12-03
draft: false
summary: "Learn to use Oracle Linux Automation Engine to perform the initial configuration and other administrative tasks for Oracle Linux."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/56b90194-88ab-421e-bc93-2ac708dce6ba)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-ol-tasks)

## Details

Oracle Linux Automation Engine enables administrators to automate the initial setup of Oracle Linux and run other administrative jobs using an Infrastructure as code (IaC) configuration management tool through a series of playbooks and tasks.

### Objectives

In this tutorial, you'll learn how to:

- Write playbooks that:
  - Create a user
  - Adds the user to the *sudo* group
  - Copies a local SSH public key to the user's *authorized_keys* file
  - Adds a DNF repository and installs a package
  - Manipulates files

### Prerequisites

- A minimum of two Oracle Linux systems with the following configuration:

  - a non-root user with *sudo* permissions
  - ssh keypair for the non-root user
  - the ability to SSH from one host to another using a passwordless SSH login

