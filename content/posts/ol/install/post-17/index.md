---
title: "Use Fedora Media Writer"
date: 2022-03-24
draft: false
summary: "Learn how to use Fedora Media Writer to create Oracle Linux installation media on a USB device with any compatible operating system."
tags: ["ol","tutorial","ol-install"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/usb-media)

## Details

Oracle Linux is distributed as an ISO image, which is a binary representation of the files and contents for installing the operating system. An Oracle Linux installation requires that you need to create an installation media from the ISO image.
As the official documentation shows, Oracle's supported method for creating the installation media is by using the dd command. However, you can choose any preferred third party utility, such as Balena Etcher or Rufus.
This tutorial focuses on using Fedora Media Writer to create installation media on a USB flash drive. If you want to create installation media from more than one ISO image on the same USB flash drive, follow the instructions in our tutorial for using Ventoy instead.
The Fedora Media Writer is a utility from the Fedora project for creating installation media primarily for Fedora Linux installations. However, it can be used for other Linux distributions as well, such as Oracle Linux. Fedora Media Writer is supported on Windows and macOS. Therefore, users of those systems can also avail of the utility to create Oracle Linux installation media.

Objectives
At the end of this tutorial, you should be able to do the following:

Download an Oracle Linux ISO.
Format the USB drive with the correct file system.
Copy the ISO image contents to the USB drive.


Prerequisites

Any system that is running Windows 10 or newer, macOS 12 or newer, or a recent Linux distribution.
A secure USB flash drive or external hard drive.