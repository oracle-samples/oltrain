---
title: "Package Management"
date: 2020-08-03
weight: 06
draft: false
description: "Package Management"
summary: "This track focusses on software package management is an essential skill needed to keep your Oracle Linux system up to date with the latest software enhancements, bug fixes, and security patches. Oracle Linux 8 introduced DNF, which replaces YUM, and in this video series, we cover how to use DNF, install the Oracle UEK kernel and how to add repositories."
tags: [ "Package Management", "DNF", "EPEL Repository" ]
slug: "pkg-mgmt"
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
- /OL/pkg_mgmt/pkg_mgmt.html
---

## Videos

{{< lead >}} Software package management is an essential skill needed to keep your Oracle Linux system up to date with the latest software enhancements, bug fixes, and security patches. Oracle Linux 8 introduced DNF, which replaces YUM, and in this video series, we cover how to use DNF, install the Oracle UEK kernel and how to add repositories. {{< /lead >}}

### DNF on Oracle Linux

- {{< youtube YP_ovje5UuM >}}

### Installing the Unbreakable Enterprise Kernel Release 6 on Oracle Linux 8

- {{< youtube OeFTjC0mqLM >}}

### Installing the EPEL Repository on Oracle Linux

- {{< youtube R-hAYGEYWQ0 >}}

## Labs

{{< lead >}} Each hands-on lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment. {{< /lead >}}

### [Use DNF on Oracle Linux](https://luna.oracle.com/lab/609f19ec-b142-4fa9-81d1-ab6d1e97478c)

Learn how to work with DNF repositories. list package information, install, download, and reinstall packages, upgrade and remove packages, use the DNF history feature, and manage package groups.

---

### [Use DNF to Maintain Security on Oracle Linux](https://luna.oracle.com/lab/b48151dc-20d9-4c52-b868-840978f4a514)

Learn to use DNF for security package maintenance on Oracle Linux.

---

### [Manage AppSteam Modules on Oracle Linux](https://luna.oracle.com/lab/19feea85-3457-4e8d-bf4d-7f962ee0505f)

Learn to manage and maintain user-space applications using AppStream modules on Oracle Linux.

---

### [Mirror a Yum Repository on Oracle Linux](https://luna.oracle.com/lab/b3779123-c17c-4f89-bb93-8c343d891825)

Learn to mirror and share a Yum repository with local, offline, or distributed systems.

The task of mirroring a yum repository holds multiple benefits. These include the following:

- Provide access to yum repositories for systems without access to a public network
- Improve software download times and reduce the bandwidth overhead of a large infrastructure
- Configure local network-based installation strategies
- Catering for a snapshot style update strategy where performing testing against a controlled software distribution environment

This lab shows how to mirror a yum repository for local, offline, or distributed systems access.

---

{{< figure src="/img/quiz1.png" alt="ol-package-mgmt-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:2EE70X" target="_blank" >}}
Take the quiz
{{< /button >}}