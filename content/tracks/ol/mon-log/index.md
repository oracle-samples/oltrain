---
title: "Monitoring and Logging"
date: 2020-08-03
weight: 08
draft: false
description: "Monitoring and Logging"
summary: "This track focusses on typical monitoring and logging tasks performed on a Linux system. Learn how to monitor system performance and review system logs on Oracle Linux."
tags: ["monitoring","logging","profiling"]
slug: "mon-log"
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
- /OL/mon_log/mon_log.html
series: ["Oracle Linux"]
series_order: 6
---

## Videos

{{< lead >}} These videos go through typical monitoring and logging tasks performed on a Linux system. Learn how to monitor system performance and review system logs on Oracle Linux. {{< /lead >}}

### Use Gprofng for Performance Profiling Applications

- {{< youtube TRZNoL_7xro >}}

### Using the sosreport Utility on Oracle Linux

- {{< youtube FD-wgH4xhJI >}}

### Using the iostat Utility on Oracle Linux

- {{< youtube BCb1Il1hpgY >}}

### Using the mpstat Utility on Oracle Linux

- {{< youtube ioAP964a_Q0 >}}

### Using the vmstat Utility on Oracle Linux

- {{< youtube WGOWGJGFlvU >}}

### Using the top Utility on Oracle Linux

- {{< youtube t3JZ8Tcw7fo >}}

### Using the netstat Utility on Oracle Linux

- {{< youtube ucWjQafk1fk >}}

### System Logging with rsyslog on Oracle Linux

- {{< youtube Xxk2bbiwr6M >}}

### System Logging with logwatch on Oracle Linux

- {{< youtube jfdcGZJIuLk >}}

### System Logging with journald on Oracle Linux

- {{< youtube YAMF3ewtfa4 >}}

### Linux Auditing System on Oracle Linux

- {{< youtube AKwV0DHt6oA >}}

## Labs

{{< lead >}} Each hands-on lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment. {{< /lead >}}

### [Monitor System Resources on Oracle Linux](https://luna.oracle.com/lab/73bf7efa-53a1-4528-ad60-5f7b721fc3f8)

Learn how to use the vmstat, mpstat and top commands to monitory system resources on Oracle Linux.

In this lab you work with the Oracle Linux vmstat, mpstat, and top to monitor system resource usage. Monitoring the usage of system resourses is useful for detecting issues which can adversely affect system performance.

---

### [System Logging on Oracle Linux](https://luna.oracle.com/lab/3f0906f5-a80e-418b-a8b4-48c60103c55c)

Learn to use journald, logwatch, and rsyslog on Oracle Linux.

In this lab, you configure system logging, use rsyslog templates to format log messages, install and run logwatch, view the journald journal, and configure persistent journald storage.

---

### [Audit Oracle Linux with Auditd](https://luna.oracle.com/lab/3a72b337-d8c0-41b9-9193-e1bf50ad2ac9)

Learn to use auditd with Oracle Linux.

Auditd is a userspace system daemon that runs in the background generating logs about different activities performed on Oracle Linux.

This lab guides you through installation, configuration, and using auditd.

---

{{< figure src="/img/quiz1.png" alt="ol-mon-log-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:CF0JMU5" target="_blank" >}}
Take the quiz
{{< /button >}}
