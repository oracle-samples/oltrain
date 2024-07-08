---
title: "Install Postfix"
date: 2021-09-10
draft: false
summary: "Learn how to install Postfix as an SMTP server and Mail Submission Agent on Oracle Linux."
tags: ["ol","tutorial","ol-admin"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-postfix)

## Details

These guides show you how to install and set up the Postfix email server software on an Oracle Linux system to enable you to send messages within your network. This tutorial is targeted at users of Oracle Linux 8 or later.

Postfix is a Mail Transfer Agent (MTA) server that was developed as a replacement for `sendmail`, which is the default MTA server on many older Linux systems. Because of its modular pipeline-based architecture, Postfix is versatile and integrates easily with many other services, such as spam and anti-virus processing, as well as with message store software, such as the Dovecot IMAP and POP server.

This tutorial describes how to set up and configure Postfix to function primarily as a Simple Mail Transfer Protocol (SMTP) server.

### Objectives

Upon completion of this Lab you will be able to:

- Set the server host name
- Install Postfix with appropriate firewall rules
- Configure Postfix to send unencrypted email
- Send test emails by using `mailx`
- Review the Postfix mail queue

### Prerequisites

- Any system with Oracle Linux 8

