---
title: "Use a Dynamic Inventory"
date: 2022-04-05
draft: false
summary: "Learn how to use an OCI Dynamic Inventory with Oracle Linux Automation Engine."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/95a9fc4b-56a4-4b89-b8f1-b90489df5340)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-dyninv)

## Details

Oracle Linux Automation Engine, the open-source software for provisioning and configuration management, uses an inventory file to work against managed nodes or hosts in your infrastructure. This inventory file contains a list of servers, their IP addresses, and other optional connection information.

A static inventory file works well if your infrastructure hardly changes.

However, your infrastructure is likely in constant flux when using the cloud. Therefore it would be great to have a way to have your inventory dynamically updated as hosts come and go.

### Objectives

In this lab, you'll learn to:

   - Setup Oracle Linux Automation Engine
   - Create an OCI Dynamic Inventory
   - Use the OCI Dynamic Inventory with a Playbook.

### Prerequisites

  - Install an Oracle Linux system with the following configuration:
      - a non-root user with `sudo` permissions


