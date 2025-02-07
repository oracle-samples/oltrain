---
title: "Manage Time and Tasks"
date: 2021-07-02
draft: false
summary: "Learn to set your system's date and time and schedule tasks using systemd timers on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/d857ff70-1799-472e-b413-32ea7e356470)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-chrony-systemd-timers)

## Details

Oracle Linux provides users with several ways to interact with the time and date. While you can change these manually, it is more common to configure a service that implements the Network Time Protocol (NTP), such as [chrony](https://chrony-project.org/). This way, your system time remains correct, and any tasks using `cron` or `systemd timers` run on schedule.

### Objectives

In this tutorial, you'll learn to:

- Manage your system time from the terminal using `date`, `hwclock`, and `timedatectl`
- Run and enable the *chrony* service
- Schedule tasks with *cron* and systemd *timers*

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account with sudo access
  - Access to the Internet
