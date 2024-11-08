---
title: "Write a Playbook"
date: 2024-11-08
draft: false
summary: "Learn to write a playbook using the Oracle Linux Automation Engine."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/27118507-76a6-4116-8ae3-eecc5314531e)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/olae-playbook)

## Details

The Oracle Linux Automation Engine, a component of Oracle Linux Automation Manager, is an automation tool for deploying software, configuring systems, and orchestrating tasks, such as upgrades and updates, in the form of playbooks. Initially using the `ansible` package, Oracle Linux Automation Engine now stems from the open-source `ansible-core` software package.

The following tutorial introduces writing playbooks with Oracle Linux Automation Engine.  

### Objectives

In this tutorial, you'll learn how to:

- Install Oracle Linux Automation Engine
- Create an inventory file
- Run an ad hoc command
- Write and run a playbook

### Prerequisites

- A minimum of two Oracle Linux systems with the following configuration:

  - a non-root user with `sudo` permissions
  - ssh keypair for the non-root user
  - the ability to SSH from one host to another using a passwordless SSH login
