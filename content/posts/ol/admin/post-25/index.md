---
title: "Install FreeIPA"
date: 2022-10-07
draft: false
summary: "Learn how to install and configure a FreeIPA Server on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/19bfac85-6c1e-4775-8fc3-6f55022a8e47)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-freeipa)

## Details

FreeIPA is an open-source identity and authentication management system for Linux networked environments. The server includes the 389 Directory Server as the central data store, providing full multi-master LDAPv3 functionality.

Beyond the scope of this tutorial, FreeIPA also provides MIT Kerberos for Single-Sign-on authentication, the Dogtag Certificate Authority, and optional Domain Name management through an ISC Bind server.

This tutorial shows how to install FreeIPA and configure the included LDAP directory.

### Objectives

In this tutorial, you will learn how to:

  - Install FreeIPA Server
  - Disable anonymous binds
  - Add Users and Groups

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - An FQDN (Fully Qualified Domain Name ) pointing to your server’s IP address

> For more information on requirements for FreeIPA, see the upstream [Quick Start Guide](https://www.freeipa.org/page/Quick_Start_Guide#Preparing_a_Platform).

