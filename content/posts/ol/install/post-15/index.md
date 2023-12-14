---
title: "Use Ventoy"
date: 2023-12-01
draft: false
summary: "Learn how to use Ventoy to create Oracle Linux installation media on a USB device with any compatible operating system."
tags: ["ol","tutorial","ol-install"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/usb-media-ventoy)

## Details

Oracle Linux is distributed as an [ISO image](https://en.wikipedia.org/wiki/ISO_image), which is a binary representation of the files and contents for installing the operating system. An Oracle Linux installation requires that you need to create an installation media from the ISO image.

As the official documentation shows, Oracle's supported method for creating the installation media is by using the `dd` command. However, you can choose any preferred third party utility, such as Balena Etcher or Rufus.

This tutorial focuses on using Ventoy to create installation media on a USB drive. If you are using macOS, follow the instructions in [our tutorial for Fedora Media Writer](https://docs.oracle.com/en/learn/usb-media/) instead.

Ventoy is a utility that creates a bootable USB device, but unlike other installation media creation tools that copy the contents of one ISO image onto one USB device, Ventoy installs a custom bootloader onto that USB media and then creates a blank partition onto which you can copy one or more ISO image files.

This approach means that, instead of needing three separate USB devices for each ISO image, you can use the same physical USB device to run install media for Oracle Linux 7, Oracle Linux 8, and Oracle Linux 9. Also, whenever Oracle releases a new ISO image, you can copy it onto your existing USB device instead of creating new install media for Oracle Linux on another USB device. You can also continue to use your USB flash drive to back up files and copy files between machines.

## Objectives

At the end of this tutorial, you should be able to do the following:

- Download one or more Oracle Linux ISO images.
- Format the USB drive with the correct file system.
- Download, install, and run Ventoy.
- Copy ISO image files to the USB drive.

## Prerequisites

- Any system that is running Windows 10 or newer, or a recent Linux distribution.
- A secure USB flash drive or external hard drive.
