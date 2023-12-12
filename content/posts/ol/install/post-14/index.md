---
title: "Switch from CentOS 8"
date: 2021-03-24
draft: false
summary: "Learn how to convert from CentOS 8 to Oracle Linux 8"
tags: ["ol","tutorial","ol-install"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/switch_centos8_linux8)

## Details

The following tutorial provides step-by-step procedures to automatically switch a CentOS 8 instance to Oracle Linux 8 by removing any CentOS-specific packages or replacing them with the Oracle Linux equivalent. As the [README.md](https://github.com/oracle/centos2ol) states in the Oracle centos2ol repository on GitHub, the script used in this tutorial is a work-in-progress and not designed to handle all possible configurations.

Please ensure you have a *complete backup* of the system before starting this process if the script cannot successfully convert the system.

Be sure to review the centos2ol project [README.md](https://github.com/oracle/centos2ol) file for the latest details.

### Objectives

In this lab, you'll:

  - Check for non-standard kernels
  - Ensure `dnf` configuration is working
  - Disable or remove stale and non-CentOS repositories
  - Ensure 5GB free space in `/var/cache`
  - Disable all automatic updates, including `dnf-automatic`

### Prerequisite

  - A system with CentOS 8 installed.

