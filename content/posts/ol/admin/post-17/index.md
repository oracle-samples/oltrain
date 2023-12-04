---
title: "Scheduling Tasks"
date: 2021-07-02
draft: false
summary: "Learn how to use the crontab command on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/d857ff70-1799-472e-b413-32ea7e356470)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-crontab)

## Details

These guides show you how to use the crontab command on Oracle Linux.

### Background

Oracle Linux can run programs automatically as scheduled tasks or jobs. You can either schedule programs to run as system-level tasks by editing cron configuration in `/etc/cron*`; or you can schedule programs to run as jobs within your user crontab. If you do not have system administrator access on a system or the programs that you wish to schedule are specific to your user account, the crontab utility provides a good mechanism to run programs on a regular schedule under your own user credentials. The crontab allows you to schedule jobs to run as often as every minute or as infrequently as once a year; however you should note that cron job will not run if the system is down during the time that the job was scheduled to run.

Note that cron configuration is standard on most Linux systems and has been available for Unix-like systems since 1975. More complex scheduling solutions are included in Systemd in the form of timers and users are encouraged to explore Systemd timers in more depth to solve specific requirements. However, this tutorial provides foundational training that is more suitable for the average user.

### What Do You Need?

- A system with Oracle Linux installed


