---
title: "System Logging"
date: 2021-11-03
draft: true
summary: "Learn how to use journald, logwatch, and rsyslog on Oracle Linux."
tags: ["ol","lab","tutorial","ol-monitor"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/3f0906f5-a80e-418b-a8b4-48c60103c55c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/system_logging_linux8)

## Details

In these guides, you configure system logging, use `rsyslog` templates to format log messages, install and run `logwatch`, view the `journald journal`, and configure persistent `journald` storage.

### Background

System log files contain messages about the system, kernel, services, and applications. The `journald` logging daemon, which is part of `systemd`, records system messages in non-persistent journal logs in memory and in the `/run/log/journal` directory. `journald` forwards messages to the system logging daemon, `rsyslog`. As files in `/run` are volatile, the log data is lost after a reboot unless you create the directory `/var/log/journal`. You can use the `journalctl` command to query the journal logs.


### Objectives

- Explore the `rsylog.conf` file
- Explore the `logrotate.conf` file
- Configure and use `rsyslog` templates
- Install `logwatch` and run the `logwatch` utility
- Explore and use `journald`

### What Do You Need?

A fully patched Oracle Linux or later system.

