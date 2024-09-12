---
title: "Build Multi-Platform Images"
date: 2021-07-29
draft: false
summary: "Learn how to build multi-platform container images using Podman on Oracle Linux."
tags: ["ol","tutorial","ol-podman"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-build-multi-platform-images)

## Details

This demo shows the creation of a multi-platform container image using Podman on Oracle Linux.

### Objectives

In this tutorial, you'll learn how to:

  - Configure Podman for remote connectivity
  - Connect to a remote Podman instance
  - Build platform-specific images from a single Containerfile
  - Push platform-specific images to the Oracle Cloud Infrastructure Registry (OCIR)
  - Create a manifest list that includes both platform-specific images
  - Push the manifest list to OCIR
  - Inspect the OCIR-hosted manifest list to see the available platforms
  - Pull and run the image

### Prerequisites

  - Access to an Oracle Cloud Infrastructure (OCI) tenancy
  - An Oracle Linux x86_64 instance
  - An Oracle Cloud Developer aarch_64 instance
  - Access to Oracle Cloud Infrastructure Registry