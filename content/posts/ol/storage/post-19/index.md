---
title: "Use Network Bound Disk Encryption"
date: 2021-06-21
draft: false
summary: "Learn how to use Network Bound Disk Encryption with Tang and Clevis on Oracle Linux."
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/e348bfed-8e08-4b12-8114-74e87eb12497)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-tang-clevis)

## Details

This tutorial demonstrates how to configure an Oracle Linux system with Linux Unified Key Setup (LUKS) disk encryption that is dependent on a network-based key service consisting of [Tang](https://github.com/latchset/tang) and [Clevis](https://github.com/latchset/clevis). You will create an encrypted XFS file system that is automatically unlocked at boot when on the same network as your key server.

### Objectives

In this tutorial, you'll learn how to:

  - Set up LUKS using [cryptsetup](https://gitlab.com/cryptsetup/cryptsetup/-/wikis/home), which provides the tooling for disk-based encryption and includes support for LUKS.
  - Configure Tang as a network service that provides cryptographic services over HTTP.
  - Use Clevis for the network encryption framework. Clevis can use keys provided by Tang as a passphrase to unlock LUKS volumes.


### Prerequisites

- Minimum of two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
    - A disk or block device attached to the system to use for encrypted storage

