---
title: "Administration"
date: 2020-08-03
weight: 09
draft: false
description: "Administration."
summary: "This covers some common administration tasks that you can perform on Oracle Linux. You can learn step-by-step how to configure the system date and time, automate tasks, dynamically load and unload kernel modules, configure users and groups, and explore the proc and sysfs file systems to view and configure system hardware and system processes. These tasks are applicable for on-premises systems or Oracle Cloud Infrastructure instances."
tags: [ "administration", "leapp", "selinux" ]
slug: "admin"
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
- /OL/admin/admin.html
series: ["Oracle Linux"]
series_order: 1
---

## Videos

{{< lead >}} These short videos go through some common administration tasks that you can perform on Oracle Linux. You can learn step-by-step how to configure the system date and time, automate tasks, dynamically load and unload kernel modules, configure users and groups, and explore the proc and sysfs file systems to view and configure system hardware and system processes. These tasks are applicable for on-premises systems or Oracle Cloud Infrastructure instances. {{< /lead >}}

### Date and Time Configuration on Oracle Linux

- {{< youtube q8VlYiF5sx8 >}}

### Proc File System on Oracle Linux

- {{< youtube 1F51ZHAVfAk >}}

### sysfs File System on Oracle Linux

- {{< youtube j9x2cuOE5_Y >}}

### Automating Tasks with Cron on Oracle Linux

- {{< youtube BpPGoRYTv9I >}}

### Automating Tasks with anacron, at, and batch on Oracle Linux

- {{< youtube EIV3lpTeqXo >}}

### Kernel Module Configuration on Oracle Linux

- {{< youtube AeW42ZyzHrQ >}}

### User and Group Administration on Oracle Linux

- {{< youtube fag6aHNUkdQ >}}

### Password Aging and su Command on Oracle Linux

- {{< youtube WrcnDpj3axQ >}}

### FTP Configuration on Oracle Linux

- {{< youtube xpBBUPLEkZg >}}

### Oracle Linux Upgrades with LEAPP

- {{< youtube kxeBILa3YNc >}}

### Introduction to Control Groups on Oracle Linux

- {{< youtube AiYK0VBW7e4 >}}

### SELinux Basics on Oracle Linux

- {{< youtube meKjLOxEu_o >}}

### Pluggable Authentication Modules (PAM) on Oracle Linux

- {{< youtube KRGC2lElVC8 >}}

### Introducing Udev on Oracle Linux

- {{< youtube y3q8HAMTPDc >}}

## Labs

---

{{< lead >}} Each hands-on lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment. {{< /lead >}}

---

### [Create users and groups on Oracle Linux](https://luna.oracle.com/lab/fb0e97c0-4522-422f-8be3-dd6f70a7b96e)

Learn to perform user and group administration, implement user private group scheme, and grant user elevated privileges.  The following lab provides step-by-step procedures to perform user and group administration on Oracle Linux. You will create users and groups, implement user private groups, and grant user elevated privileges.

---

### [Configure Chrony on Oracle Linux](https://luna.oracle.com/lab/4946609e-41e4-4d26-8501-da948bb299ba)

Learn to set date, time and configure Network Time Protocol using Chrony.  The following lab provides step-by-step procedures to configure date and time, and enable Chrony. This lab is targeted at Oracle Linux 8 users, but the commands are also available on other Oracle Linux releases.

---

### [Use the Crontab Utility to Schedule Tasks on Oracle Linux](https://luna.oracle.com/lab/d857ff70-1799-472e-b413-32ea7e356470)

This lab shows you how to use the crontab command on Oracle Linux.  

Oracle Linux can run programs automatically as scheduled tasks or jobs. You can either schedule programs to run as system-level tasks by editing cron configuration in /etc/cron*; or you can schedule programs to run as jobs within your user crontab. If you do not have system administrator access on a system or the programs that you wish to schedule are specific to your user account, the crontab utility provides a good mechanism to run programs on a regular schedule under your own user credentials. The crontab allows you to schedule jobs to run as often as every minute or as infrequently as once a year; however you should note that cron job will not run if the system is down during the time that the job was scheduled to run.

---

### [Use tmux on Oracle Linux](https://luna.oracle.com/lab/4dda7413-1a31-47bf-96c1-8fa6c306dc6b)

Learn how to use tmux to control multiple terminal windows in a persistent session on Oracle Linux.  This lab provides step-by-step procedures for controlling multiple terminal windows in the same persistent session.

By default, terminating your SSH connection also terminates any remote terminal sessions started by that connection. If you use a terminal multiplexer, you can preserve those sessions for yourself and others to reuse. You can also manage more complex tasks from a single SSH connection, as a terminal multiplexer can provide browser-style tabs for each task, and even divide up your screen with multiple terminal sessions called "panes".

---

### [Install and Configure Postfix on Oracle Linux](https://luna.oracle.com/lab/4255c51c-4f52-45f3-a3e8-125b8cf1b40b)

Learn how to install Postfix as an SMTP server and Mail Submission Agent on Oracle Linux.

This lab shows you how to install and set up the Postfix email server software on an Oracle Linux system to enable you to send messages within your network. This lab is targeted at users of Oracle Linux 8 or later.

Postfix is a Mail Transfer Agent (MTA) server that was developed as a replacement for sendmail, which is the default MTA server on many older Linux systems. Because of its modular pipeline-based architecture, Postfix is versatile and integrates easily with many other services, such as spam and anti-virus processing, as well as with message store software, such as the Dovecot IMAP and POP server.

This tutorial describes how to set up and configure Postfix to function primarily as a Simple Mail Transfer Protocol (SMTP) server.

---

### [Configure STARTTLS for Postfix on Oracle Linux](https://luna.oracle.com/lab/6c0d44b2-1247-4780-a1ae-09f283812ef8)

Learn how to install Postfix as an SMTP server and Mail Submission Agent with STARTTLS on Oracle Linux.

This lab shows you how to install and set up the Postfix email server software on an Oracle Linux system to enable you to send messages within your network with STARTTLS encryption and verification. This lab is targeted at users of Oracle Linux 8 or later.

Postfix is a Mail Transfer Agent (MTA) server that was developed as a replacement for sendmail, which is the default MTA server on many older Linux systems. Because of its modular pipeline-based architecture, Postfix is versatile and integrates easily with many other services, such as spam and anti-virus processing, as well as with message store software, such as the Dovecot IMAP and POP server.

As a bare minimum to secure the service, you should configure Postfix to support STARTTLS to perform TLS/SSL verification and encryption over an SMTP connection. Using STARTTLS helps to protect the integrity of your communications.

---

### [Install the NGINX Web Server and Proxy on Oracle Linux](https://luna.oracle.com/lab/54fa9d88-4243-4b4f-bae2-d52ec8cfb688)

Learn how to install the NGINX web server and enable it in Oracle Linux.

NGINX is a lightweight HTTP/S server that is capable of higher performance and lower memory use than a typical Apache web server deployment. However, this performance gain comes at the cost of some functionality and flexibility. NGINX has also gained in popularity as a powerful proxy service that is capable of functioning as a direct HTTP proxy, a reverse proxy with caching, an SMTP, POP3 or IMAP proxy or as a generic TCP/UDP proxy. NGINX also provides load balancing services with fault tolerance.

On earlier Oracle Linux versions, the NGINX web server was provided as part of a software collection package. The web server package is now directly available from the Oracle Linux 8 Application Streams repository and therefore simpler to deploy and configure.

---

### [Upgrade Oracle Linux with Leapp](https://luna.oracle.com/lab/908d0e5b-4444-400a-87a7-2a9ec8c27550)

Learn how to use the Leapp utility to upgrade an Oracle Linux 7 system to Oracle Linux 8.

The Leapp utility is a framework for updating and upgrading operating systems as well as applications. The utility's component packages enable the creation of different workflows into profiles for updating software.

Leapp operations consist of two phases:

- Preupgrade - a process that examines many aspects of the system and runs checks to determine if the OS software can be upgraded.
- Upgrade - updates the system based on configuration files that map packages between previous and current versions of the software.

---

### [Run Control Groups Version 2 on Oracle Linux](https://luna.oracle.com/lab/14d89b6d-627b-4f1f-b859-4761e3ed352c)

Learn how to enable control groups (cgroups) v2 and limit the CPU time for user slices.

Control Groups (cgroups) is a Linux kernel feature for limiting, prioritizing, and allocating resources such as CPU time, memory, and network bandwidth for running processes.

---

### [Use SELinux on Oracle Linux](https://luna.oracle.com/lab/89a09fdd-47c2-4755-b98e-35863bdf7bc0)

Learn how to use SELinux on Oracle Linux.

SELinux is a set of kernel mods and user-space tools that provide another layer of system security, precise access control, system-wide admin-defined policies, and improved mitigation for privilege escalation attacks.

This lab guides you through using these user-space tools to help keep your system running in enforcing mode.

---

### [Install FreeIPA Server on Oracle Linux](https://luna.oracle.com/lab/19bfac85-6c1e-4775-8fc3-6f55022a8e47)

Learn how to install and configure a FreeIPA Server on Oracle Linux.  FreeIPA is an open-source identity and authentication management system for Linux networked environments. The server includes the 389 Directory Server as the central data store, providing full multi-master LDAPv3 functionality.  

Beyond the scope of this lab, FreeIPA also provides MIT Kerberos for Single-Sign-on authentication, the Dogtag Certificate Authority, and optional Domain Name management through an ISC Bind server.

This lab shows how to install FreeIPA and configure the included LDAP directory.

---

### [Deploy Keycloak using Podman on Oracle Linux](https://luna.oracle.com/lab/752793ff-9f74-4bb0-b848-90c5bcae4388)

Learn to deploy Keycloak for providing authentication to applications and secure services using OAuth and SAML.

Keycloak provides single sign-on functionality for web applications and RESTFUL web services. A primary goal of Keycloak is to provide security features that developers can easily use to secure applications and services within their organizations, for example Single-Sign-On authentication. Keycloak can also be integrated with existing LDAP and Active Directory servers.

Keycloak is based on standard protocols and provides support for User Federation, OpenID Connect, OAuth 2.0 and SAML and many more. Keycloak provides both administrators, and users, with management consoles. Users can update their passwords, profile details and setup two-factor authentication via the Account Management Console. Likewise administrators can use the Admin Console to manage all aspects of Keycloak's functionality, it's authorization policies, applications and manage users (including user's permissions and sessions).

---

### [Get Started with Oracle Database Free on Oracle Linux](https://luna.oracle.com/lab/8dd46cea-3e27-4774-bb12-fc97a4babe06)

Learn to install the Oracle Database Free on Oracle Linux.

Oracle Database Free—Developer Release is the same powerful Oracle Database businesses worldwide rely on. It offers a full-featured experience and is packaged for ease of use and simple download—for free.

Whether you are a developer, a data scientist, a DBA, an educator, or just interested in databases, Oracle Database 23c Free—Developer Release is the ideal way to get started. It provides native support for all modern data types, analytics, and the latest development paradigms—all built into one product.

This lab uses the container and RPM installation methods to install Oracle Database Free on Oracle Linux.

---

### [Disable a Kernel Module on Oracle Linux](https://luna.oracle.com/lab/00aafe17-39b9-43e0-8b53-087b84003c15)

Disable a Kernel Module on Oracle Linux.

In this lab you unload a kernel module on an Oracle Linux instance and configure the system to prevent the module from loading at boot time. You can use this knowledge to disable kernel modules for hardware that might be causing a problem on a system or that may be flagged for a vulnerability.

---

### [Use ReaR to Perform an Oracle Linux Backup](https://luna.oracle.com/lab/30023183-ca96-48dc-8497-af04ca1eada4)

Learn how to perform a backup of Oracle Linux using the ReaR disaster recovery solution.

Relax-and-Recover (ReaR) was born in 2006 by Gratien D'haese and Schlomo Schapiro as part of a complete rewrite of an earlier Linux Disaster Recovery project mkCDrec. ReaR is an Open Source bare metal disaster recovery solution that Oracle Linux (OL) provides natively. It produces a bootable image that can recreate the system's original storage layout and restore from the backup.

ReaR is directly available from the Application Streams repository in Oracle Linux 8 or later and is simple to deploy and configure.

This lab guides users on installing and configuring ReaR to backup and restore Oracle Linux using NFS storage.

---

### [Install Oracle Java SE on Oracle Linux](https://luna.oracle.com/lab/00f34840-f6d0-47dc-9a83-0cc6abd5d051)

Oracle's Java Platform , Standard Edition (Java SE ) lets you develop and deploy Java applications on desktops and servers.

The Java Platform Standard Edition Development Kit (JDK) includes tools for developing, testing, and monitoring programs written in the Java programming language and running on the Java platform. The JDK offers developers and users a rich user interface and the performance, versatility, portability, and security that today's applications require.

Beyond these great features, Oracle provides the Oracle JDK free for commercial and production use. When you combine Oracle Java with Oracle's highly performant, reliable, and cloud-ready operating system, Oracle Linux , you get an ideal environment with out-of-the-box optimizations for Oracle software, excellent for running Oracle Java.

---

### [Run Oracle Database on Oracle Linux for Arm](https://luna.oracle.com/lab/2a32f4bb-2cd1-4f9f-a900-db8f147c0b14)

Oracle Database 19c Enterprise Edition, the current long-term support release of Oracle Database, is now certified and available on the popular Arm architecture for cloud and on-premises deployments.

The Oracle Cloud Infrastructure (OCI) Ampere A1 compute platform provides deterministic performance, linear scalability, and an energy-efficient, sustainable, eco-friendly design for Oracle Database customers. Building applications is free to try, easy to learn, and fast to explore.

---

### [Get Started with Git on Oracle Linux](https://luna.oracle.com/lab/6c55a20f-e751-4326-a157-b16770262346)

Git is a free and open-source Distributed Version Control System (DVCS) which is available for MacOS, MS Windows and Linux/Unix platforms. This lab only covers using Git on Oracle Linux, but the steps covered in this lab work for any platform.

How does Git work? Git does not need a centrally located Git server to be fully functional. Instead, a simple project consists of a local folder on your computer containing files. Git then tracks any changes made to the directories and files contained within the project over time. It achieves this by storing the history and details of branches and commits locally without requiring a network connection.

---

{{< figure src="/img/quiz1.png" alt="ol-admin-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:IJY13J" target="_blank" >}}
Take the quiz
{{< /button >}}