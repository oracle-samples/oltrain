---
title: "Build Multi-Platform Images"
date: 2021-07-29
draft: false
summary: "Learn how to create multi-platform container images using Podman on Oracle Linux."
tags: ["ol","tutorial","ol-podman"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-platform-images)

## Details

This demo shows the creation of a multi-platform container image using Podman on Oracle Linux.

### Objectives

In this lab, you'll:

  - Configure Podman for remote connectivity
  - Connect to a remote Podman instance
  - Build platform-specific images from a single Containerfile
  - Push platform-specific images to the Oracle Cloud Infrastructure Registry (OCIR)
  - Create a manifest list that includes both platform-specfic images
  - Push the manifest list to OCIR
  - Inspect the OCIR hosted manifest list to see the available platforms.
  - Pull and run the image

### What Do You Need?

  - An Oracle Cloud Infrastructure tenancy
  - An x86_64 system with Oracle Linux 8 or later installed
  - An aarch_64 system with Oracle Cloud Developer installed

