---
title: "Switch from CentOS 7"
date: 2022-11-14
draft: false
summary: "Learn how to convert from CentOS 7 to Oracle Linux 7"
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/660a07d9-0580-4fae-973b-d5dfaebda1cb)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/switch_centos7_ol7)

## Details

The following guides provide step-by-step procedures to automatically switch a CentOS 7 instance to Oracle Linux 7 by removing any CentOS-specific packages or replacing them with the Oracle Linux equivalent. As the [README.md](https://github.com/oracle/centos2ol) states in the Oracle centos2ol repository on GitHub, the script used in this tutorial is a work-in-progress and not designed to handle all possible configurations.

Please ensure you have a *complete backup* of the system before starting this process if the script cannot successfully convert the system.

Be sure to review the centos2ol project [README.md](https://github.com/oracle/centos2ol) file for the latest details.

### Objectives

In this lab, you'll:

  - Check for non-standard kernels
  - Ensure `yum` configuration is working
  - Disable or remove stale and non-CentOS repositories
  - Ensure 5GB free space in `/var/cache`
  - Disable all automatic updates, including `yum-cron`

### Prerequisite

  - A system with CentOS 7 installed.

