---
title: "Use Custom Execution Environments"
date: 2024-01-11
draft: false
summary: "Learn to deploy and configure a custom execution environment in Oracle Linux Automation Manager for running jobs."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/9b8e3edf-72c0-4e01-9b66-b27eb1002a47)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-use-custom-ee)

## Details

Using a custom execution environment (ee), Oracle Linux Automation Manager can leverage playbooks containing collections and other resources not available with the default *olam-ee* image. You build it using the Builder utility, store it on Private Automation Hub, and then pull it into Oracle Linux Automation Manager.

How does that all work together? 

This tutorial shows how to upload a pre-built image to Private Automation Hub and then pull it into Oracle Linux Automation Manager to run playbooks. For details on creating customized execution environments, see our [tutorial](https://docs.oracle.com/en/learn/olam-builder-custom) on the Builder utility, and this [tutorial](https://docs.oracle.com/en/learn/olam-pah-manage-ee) on Private Automation Hub.

### Objectives

In this tutorial, you'll learn how to:

- Push a custom ee to Private Automation Hub using a playbook
- Add a custom ee to Oracle Linux Automation Manager
- Use the custom ee to run a Job

### Prerequisites

- Three systems running Oracle Linux
  - A development environment using the Builder utility
  - One for Private Automation Hub
  - Another for running Oracle Linux Automation Manager
