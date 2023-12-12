---
title: "NetworkManager and IP"
date: 2021-09-17
draft: false
summary: "Learn to use NetworkManager and the IP Command to configure and manage network interfaces on Oracle Linux."
tags: ["ol","lab","tutorial","ol-network"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6cbaab1f-835c-445e-89eb-b42ba3e679bb)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-nmcli)

## Details

In these guides you work with the Oracle Linux CLI utilities, `nmcli` and `ip`, to monitor and manage network devices and connections.

The intent is to introduce you to these utilities and practice using their common features to simulate a work environment. Not all of the features are presented. The lab runs in a virtualized environment and therefore limits what can be presented and practiced.

### Background

Linux handles network communications through software configuration files and the physical
networking devices in your system. Each physical network device has an associated configuration
file, named `ifcfg-<interface>`, located in the `/etc/sysconfig/network-scripts` directory.

NetworkManager includes a command-line utility, `nmcli`, which you can use to create, display, edit, delete, activate, and deactivate network connections, as well as control and display network device status.

The `ip` is another utility for displaying and manipulating network devices, network routing, and tunnels.

### Objectives

- View network status information using command line utilities: `nmcli` and `ip`.
- Change the system host name
- Change the logging level
- View connection information
- Add, edit and delete a connection profile
- View device status information

### What Do You Need?

A client system with Oracle Linux installed with at least three disk devices.

