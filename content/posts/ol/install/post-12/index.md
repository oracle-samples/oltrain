---
title: "Use Systemd"
date: 2021-06-23
draft: false
summary: "Learn to use systemd to manage system services in system and user space."
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/8a060473-bff3-4c04-9799-eb944951007c)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/ol-systemd)

## Details

Systemd is a collection of software components that manages Oracle Linux system services and settings. During system startup, the boot process initializes as *PID 1*, which *systemd* later manages. From there, *systemd* or one of its child processes starts all subsequent processes. Just like it is the first process to start after the system boots, it is the last to finish running when shutting down the system. Administrators and users use `systemctl` as the primary management tool to interact with *systemd* services and `journalctl` for troubleshooting. 

Within *systemd*, different types of *units* manage various types of system behavior or functions. For example, daemon processes or system services are run as service units, while target units usually define system states. You also have timer units to schedule tasks, similar to how you might use the system cron service, and mount units to configure a mount point instead of configuring it in the system fstab.

While *systemd* manages all system-level processes and functions, it can also manage processes running in user space. Users can manage services and timers they create without administrator access and even configure them to continue after the user session has terminated.

### Objectives

In this tutorial, you'll learn to:

- Discover different systemd unit types
- Use systemd target units
- Run various systemctl commands
- Configure systemd to allow user space processes to run after logout

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account
