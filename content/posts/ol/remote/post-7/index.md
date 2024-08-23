---
title: "Configure SSH Tunnels"
date: 2022-07-09
draft: false
summary: "Learn how to configure SSH tunnels to establish secure connections using Oracle Linux."
tags: ["ol","lab","tutorial","ol-remote"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/d1dc0830-fe30-48d4-8e5c-d30ad525e36e)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-ssh-tunnels)

## Details

SSH is the default standard for making secure connections or file transfers over an untrusted network. SSH tunneling or SSH port forwarding allows for the encapsulation of specific TCP data traffic during transit without the fear of it being eavesdropped or intercepted. This approach even allows for adding network security to legacy applications that do not natively support encryption.

### Objectives

In this tutorial, you will learn how to:

   - Create a dynamic port forwarding tunnel
   - Establish a local port forwarding tunnel

### Prerequisites

- Minimum of two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Key-based SSH, also known as password-less SSH, between the hosts
    - Access to the Internet

> This tutorial uses the Cockpit web-based application to test the SSH tunnel, available by default on Oracle Linux cloud images. You can also use VNC services or other web applications and services just as easily.
