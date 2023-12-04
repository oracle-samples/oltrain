---
title: "Use Systemd"
date: 2021-06-23
draft: false
summary: "Learn to use systemd in Oracle Linux"
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/8a060473-bff3-4c04-9799-eb944951007c)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/use_systemd)

## Details

In these guides, you learn how to use the **systemctl** command line utility to manage and view systemd units that are controlled by systemd. This tutorial is targeted at users of Oracle Linux 8 or later.

systemd is the first process that starts at boot and is the final process to terminate at system shutdown. systemd is primarily used to manage system services or processes and system initialization at boot. However, systemd is also capable of handling many other tasks and functions as well including event logging, device management, user login, task scheduling, time synchronization and system boot. Many features in systemd are not fully utilized as users may be more comfortable with alternate software for these purposes or different Linux distributions may have preferred approaches to system configuration.

Different types of behaviour or functions within systemd are handled in systemd units. For example, daemon processes or system services are run as service units, while system states are usually defined as target units. Timer units can be defined to schedule tasks similarly to how you might use the system cron service and a mount unit can be used to configure a mount point similarly to how you might configure a mount point in the system fstab.

systemd is used to manage system level processes and functions, but it is also capable of managing processes running in user space. Users on a system can configure and manage their own services and systemd can even be configured to allow these services to continue running after the user has terminated their session.

### Objectives

  - Discover different systemd unit types
  - Use systemd target units
  - Learn common **systemctl** command syntax
  - Create your own systemd timer unit in user space
  - Configure systemd to allow user space processes to run after logout

### What Do You Need?

  - A system with Oracle Linux installed.

