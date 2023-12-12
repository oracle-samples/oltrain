---
title: "Configure Podman Containers"
date: 2021-11-05
draft: false
summary: "Learn how to use Oracle Linux Automation Engine to deploy Podman Containers on Oracle Linux."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6154cf89-6a6e-45b3-98ad-635979b953e8)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-podman)

## Details

These links will guide you through creating a playbook for installing Podman and running an Oracle Linux container using the configuration management tool Oracle Linux Automation Engine.

> *Before proceeding:* If you are not familiar with running playbooks, check out our introduction tutorial, [Write a Playbook with Oracle Linux Automation Engine](https://docs.oracle.com/en/learn/olae-playbook/index.html#introduction).

When running playbooks, Oracle Linux Automation Engine runs the tasks on machines matching the `hosts` directive in the playbook. These hosts are typically defined in an `inventory` file and can either be remote or local. For these guides, we'll demonstrate how to run a playbook locally.

### Objectives

In this lab, you'll learn to:

   - Run playbooks locally
   - Add a collection to a playbook
   - Install Podman
   - Pull and run an `oraclelinux:8` container

### Prerequisites

  - An Oracle Linux system with the following configuration:

      - a non-root user with `sudo` permissions
      - install Oracle Linux Automation Engine

