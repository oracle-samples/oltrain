---
title: "Encrypt drives using LUKS"
date: 2022-07-25
draft: false
summary: "Learn how to encrypt drives using LUKS"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/9c62956d-153b-4e93-84b0-0b2759f7e4bb)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-luks/)

## Details

Oracle Linux includes device mapper crypt (`dm-crypt`) and the Linux Unified Key Setup (LUKS) to handle encryption on block devices.

In this lab, we'll focus on the front-end tools to encrypt a device using LUKS, which utilizes the `dm-crypt` module from the device mapper support included with the Linux Kernel.

### Objectives

In this tutorial, you will learn how to:

- Install `cryptsetup`
- Create an encrypted volume
- Mount an encrypted volume

### Prerequisites

The tutorial uses the following system:

- A system with an available disk and a fully patched installation of Oracle Linux.
