---
title: "Welcome to the OS Management on Oracle Cloud Infrastructure Track"
date: 2020-08-03
draft: false
description: "Welcome to OS Management on Oracle Cloud Infrastructure Track"
summary: The OS Management Service allows you to manage updates and patches for the operating system environment on your Oracle Cloud Infrastructure instances. The OS Management Service also provides options for discovering and monitoring resources on your instances."
tags: ["OSMS", "OS Management on Oracle Cloud Infrastructure" ]
slug: "osms"
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
- /OSMS/osms.html
---

{{< figure src="/img/osms/osms-page-header-1200x200.png" alt="OS Management on Oracle Cloud Infrastructure Track" >}}

---

{{< lead >}} The Oracle Cloud Infrastructure OS Management service allows you to manage and monitor updates and patches for the operating system environments on your Oracle Cloud instances, including instances managed by the OS Management Oracle Autonomous Linux service. OS Management also provides options for discovering and monitoring resources on your instances. {{< /lead >}}

---

{{< figure src="/img/osms/osms-install-section.png" alt="OS Management on Oracle Cloud Infrastructure Track" >}}

## OS Management Installation

One of the first requirements to use the OS Management Service is to have a running instance of Linux or Windows.

### Videos
 
<!-- #### Create a Linux Instance on Oracle Cloud Infrastructure

- {{< youtube tlwlLd4GvCc >}}

#### Create a Windows Instance on Oracle Cloud Infrastructure

- {{< youtube 8SgkZTUKwFg >}} -->

#### Installing Patches with OS Management for Windows in Oracle Cloud Infrastructure

- {{< youtube 4eDTl5fPNKA >}}

#### Accessing Windows Instance in Oracle Cloud Infrastructure

- {{< youtube d1fgBuE1GMY >}}

---

{{< figure src="/img/osms/osms-work-section.png" alt="OS Management on Oracle Cloud Infrastructure Track" >}}

## OS Management Usage and Configuration

These videos will provide information to get started and work with the OS Management Service on Linux and Windows instances.

### Videos

#### Getting started with OS Management for Linux on Oracle Cloud Infrastructure

- {{< youtube 7qmy5VusYKA >}}

#### Using OS Management for Linux on Oracle Cloud Infrastructure

- {{< youtube txStsCT1onc >}}

#### Working with Software Sources in OS Management

- {{< youtube zPnfHO8cu-E >}}

#### Oracle Autonomous Linux with OS Management in Oracle Cloud Infrastructure

- {{< youtube Mt_zmEJ1UtM >}}

#### Migrate Standalone Oracle Autonomous Linux Instances to OS Management Service

- {{< youtube vNY4jelIdgk >}}

#### Getting Started with OS Management for Windows in in Oracle Cloud Infrastructure

- {{< youtube DpAE_RhmRWg >}}

#### Managing Oracle Linux Module Streams and Profiles with the OS Management Service

- {{< youtube y-dnguUNr6Y >}}

#### Creating a Compliance Report with OS Management for Linux for Oracle Cloud Infrastructure

- {{< youtube _pKnAcA7GUs >}}

---

### Labs

Practice your skills with the OS Management Service with these free hands on labs.

---

#### [Migrate Standalone Oracle Autonomous Linux Instances to use OS Management Service](https://luna.oracle.com/lab/8848ec22-81cd-46d5-aeab-dd2dae36118b)

Practice using a migration script to migrate older Oracle Autonomous Linux instances to integrate with the OS Management service in Oracle Cloud Infrastructure.

Standalone Autonomous Linux instances are instances created with older Oracle Autonomous Linux images, typically from July 2021 and earlier.  These instances are referred to as standalone because, when created, they are not integrated by default with the OS Management service in Oracle Cloud Infrastructure.  An alx-migrate script has been created to migrate these standalone instances to be managed by the OS Management service. Oracle Autonomous Linux instances built with images from August 2021 onwards are by default integrated with the OS Management service.  After the script is installed, the migration can be performed, and the instance registered and then managed using the OS Management service. It then takes advantage of the additional autonomous capabilities provided by the service, such as monitoring processes and critical events, and automatic daily updating and patching.

---

#### [Managing Oracle Linux Module Streams and Profiles with the OS Management service](https://luna.oracle.com/lab/6abfafd9-749e-4b28-93ea-830b6046501d)

Oracle Linux AppStreams introduced the concept of modules, streams and profiles that allow for the management of different versions of software applications within a single OS release. From the Oracle Cloud Infrastructure console the OS Management service can manage instance modules and AppStreams, including viewing module information and updating modules, streams, and profiles. Similarly, from the command line, AppStreams on a single instance can also be installed and managed.
