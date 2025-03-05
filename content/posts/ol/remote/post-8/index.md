---
title: "Install VNC Server"
date: 2025-03-04
draft: false
summary: "Learn to install the VNC remote access server and enable it in Oracle Linux."
tags: ["ol","lab","tutorial","ol-remote"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4a0b9653-a029-4278-9987-362cccf4b384)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/install-vnc-oracle-linux)

## Details

Virtual Network Computing (VNC) is a graphical desktop-sharing system that controls remote machines by sending keyboard and mouse events over the network. VNC is particularly useful for remotely controlling Oracle Linux servers that have a graphical desktop environment installed.

You can connect to a VNC server using any compatible software client. VNC is suitable for thin client computing where multiple dumb terminals can share the same hardware resources hosted on an Oracle Linux server.

This tutorial uses TigerVNC to illustrate how to connect to systems remotely. However, you can use a different VNC software of your choice. There is a list of alternative software choices at the end of the tutorial.

TigerVNC Server was rebased from 1.9.0 to 1.10.1 in Oracle Linux 8 Update 3. This newer version is configured differently from previous versions and no longer requires the creation of systemd unit files. The instructions provided here expect you to use the latest version of Oracle Linux and its packages.

> **Note:** TigerVNC Server is available in Oracle Linux 8 and is deprecated in Oracle Linux 9.

### Objectives

In this tutorial, you'll learn to:

- Install a graphical desktop environment along with the VNC service
- Set the VNC Password for a user on the system
- Configure the VNC service for a specific user
- Start and enable the VNC service across subsequent boots
- Access the VNC server from a remote client, either directly or using an SSH tunnel
- Optionally enable x509 encryption for direct VNC access
- Optionally create firewall rules to allow direct VNC access

### Prerequisite

- Any system with the latest Oracle Linux installed
- Client software such as [TigerVNC](https://tigervnc.org/)
