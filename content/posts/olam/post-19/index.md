---
title: "Use the AWX Collection"
date: 2023-11-09
draft: false
summary: "Learn to add and manage resources in Oracle Linux Automation Manager using a playbook."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4f6fa421-09ef-448b-a0c2-5d7563146179)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-awx-collection)

## Details

The AWX Ansible Collection allows administrators to interact with Oracle Linux Automation Manager through playbooks. The modules include the ability to perform tasks such as user and group administration, creating projects, and running jobs.

This tutorial provides details on how to deploy a DevOps instance for running the playbooks and another instance with the installation of Oracle Linux Automation Manager.

### Objectives

In this lab, you'll learn how to:

  - Deploy the DevOps and Oracle Linux Automation Manager instances
  - Setup the config file on the DevOps instance
  - Write a playbook to create the required items to run a Job
  - Test and verify the playbook

### Prerequisites

  - Two systems running Oracle Linux
    - A development environment for running the AWX Ansible Collection playbooks
    - Another for running Oracle Linux Automation Manager