---
title: "Installation and Boot Process"
date: 2020-08-03
weight: 10
draft: false
description: "Installation and Boot Process."
summary: "This track focusses on the installation and boot process. You can learn step-by-step how to complete an Oracle Linux installation for on-premises deployment and how to create an Oracle Linux instance on Oracle Cloud Infrastructure. You can also learn about the boot process and how to configure different services to start at boot time."
tags: [ "Install", "Boot", "GRUB", "UEFI", "systemd" ]
slug: "inst_boot"
showRecent: false
showDate: false
showLikes: false
showViews: false
showEdit: false
showReadingTime: false
showAuthor: false
showDateUpdated : false
sharingLinks : false
cascade:
  showDate: false
  showAuthor: false
  invertPagination: true
aliases:
- /OL/inst_boot/inst_boot.html
---

## Videos

{{< lead >}} These videos focus on the installation and boot process. You can learn step-by-step how to complete an Oracle Linux installation for on-premises deployment and how to create an Oracle Linux instance on Oracle Cloud Infrastructure. You can also learn about the boot process and how to configure different services to start at boot time. {{< /lead >}}

### Installing Oracle Linux 9

- {{< youtube BDmBtP4Y7Wg >}}

### Installing Oracle Linux 8

- {{< youtube l6fapYCHaQ0 >}}

### Installing Oracle Linux 8 on Oracle Cloud Infrastructure

- {{< youtube ETpaOwAcB7M >}}

### BIOS Firmware Bootloader Process on Oracle Linux

- {{< youtube NP9BHTjih7g >}}

### GRUB 2 Bootloader on Oracle Linux

- {{< youtube 0dv87RFGcKI >}}

### Unified Extensible Firmware Interface (UEFI) on Oracle Linux

- {{< youtube OVeso8h5HZA >}}

### sytemd System and Service Manager on Oracle Linux

- {{< youtube 9uDvnZKhU8A >}}

### sytemd Target Units on Oracle Linux

- {{< youtube Tkxs-wfZrnw >}}

## Labs

{{< lead >}} Each hands-on lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment. {{< /lead >}}

### [Manage the Boot Kernel for Oracle Linux](https://luna.oracle.com/lab/67f106f2-8c50-442c-b24f-108b806be84f)

Learn how to manage the boot kernel in Oracle Linux.  This lab describes how to set the default kernel of an Oracle Linux system from the command line. This lab is targeted at Oracle Linux 8 users, but the commands are also available on other Oracle Linux releases.

---

### [Learn How to Localize Your Installation on Oracle Linux](https://luna.oracle.com/lab/d657ae3c-ac29-4b0a-943e-e533f2e8093b)

Learn how to change your hostname, time zone, and locale settings on Oracle Linux.  Many Oracle Linux systems are installed without a desktop environment. However, multiple ways of using the command line are available to configure base system settings, such as the system hostname.  This lab describes how to configure the system hostname, locale, language, and date and time from the command line. This lab is targeted at users of Oracle Linux or later.

---

### [Configure System Settings on Oracle Linux](https://luna.oracle.com/lab/aa8f2377-7967-4e45-bf32-bdc8054d5c76)

Learn to use sysctl and explore /proc, /sys and /etc/sysconfig.  The lab provides step-by-step procedures to modify system configuration files, view and modify kernel settings, and discover hardware device and device driver attributes. This lab is targeted at users of Oracle Linux 8 or later.

---

### [Use systemd on Oracle Linux](https://luna.oracle.com/lab/8a060473-bff3-4c04-9799-eb944951007c)

Learn how to use and manage systemd target units to control boot-up synchronization, service units to control services and processes, and timer units to trigger events.

In this tutorial, you learn how to use the **systemctl** command line utility to manage and view systemd units that are controlled by systemd. This tutorial is targeted at users of Oracle Linux 8 or later.

systemd is the first process that starts at boot and is the final process to terminate at system shutdown. systemd is primarily used to manage system services or processes and system initialization at boot. However, systemd is also capable of handling many other tasks and functions as well including event logging, device management, user login, task scheduling, time synchronization and system boot. Many features in systemd are not fully utilized as users may be more comfortable with alternate software for these purposes or different Linux distributions may have preferred approaches to system configuration.

Different types of behaviour or functions within systemd are handled in systemd units. For example, daemon processes or system services are run as service units, while system states are usually defined as target units. Timer units can be defined to schedule tasks similarly to how you might use the system cron service and a mount unit can be used to configure a mount point similarly to how you might configure a mount point in the system fstab.

systemd is used to manage system level processes and functions, but it is also capable of managing processes running in user space. Users on a system can configure and manage their own services and systemd can even be configured to allow these services to continue running after the user has terminated their session.

---

### [Switch from CentOS 7 to Oracle Linux 7](https://luna.oracle.com/lab/660a07d9-0580-4fae-973b-d5dfaebda1cb)

Learn how to switch a CentOS 7 instance to Oracle Linux 7.  The following lab provides step-by-step procedures to automatically switch a CentOS 7 instance to Oracle Linux 7 by removing any CentOS-specific packages or replacing them with the Oracle Linux equivalent. As the README.md states in the Oracle centos2ol repository on GitHub, the script used in this lab is a work-in-progress and not designed to handle all possible configurations.

---

## Tutorials

### [Switch from CentOS 8 to Oracle Linux 8](https://docs.oracle.com/en/learn/switch_centos8_linux8/index.html)

The following tutorial provides step-by-step procedures to automatically switch a CentOS 8 instance to Oracle Linux 8 by removing any CentOS-specific packages or replacing them with the Oracle Linux equivalent. As the README.md states in the Oracle centos2ol repository on GitHub, the script used in this tutorial is a work-in-progress and not designed to handle all possible configurations.

---

{{< figure src="/img/quiz1.png" alt="ol-inst-boot-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:DLCZA6M" target="_blank" >}}
Take the quiz
{{< /button >}}

