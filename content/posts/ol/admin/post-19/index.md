---
title: "STARTTLS for Postfix"
date: 2021-09-23
draft: false
summary: "Learn how to install Postfix as an SMTP server and Mail Submission Agent with STARTTLS on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-postfix-starttls)

## Details

These guides show you how to install and set up the Postfix email server software on an Oracle Linux system to enable you to send messages within your network with STARTTLS encryption and verification. This tutorial is targeted at users of Oracle Linux 8 or later.

Postfix is a Mail Transfer Agent (MTA) server that was developed as a replacement for `sendmail`, which is the default MTA server on many older Linux systems. Because of its modular pipeline-based architecture, Postfix is versatile and integrates easily with many other services, such as spam and anti-virus processing, as well as with message store software, such as the Dovecot IMAP and POP server.

As a bare minimum to secure the service, you should configure Postfix to support STARTTLS to perform TLS/SSL verification and encryption over an SMTP connection. Using STARTTLS helps to protect the integrity of your communications.

This tutorial describes how to set up and configure Postfix to function primarily as a Simple Mail Transfer Protocol (SMTP) server.

### Objectives

Upon completion of this Lab you will be able to:

- Set the server host name
- Install Postfix with appropriate firewall rules
- Generate a self-signed TLS certificate
- Configure Postfix to send emails and verify integrity with STARTTLS
- Send test emails by using `mailx`
- Review the Postfix mail queue

### Prerequisites

- Any system with Oracle Linux 8

