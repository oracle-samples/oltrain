---
title: "Using Compose Files"
date: 2023-01-20
draft: false
summary: "Learn to install podman-compose and use compose files with Podman on Oracle Linux."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/0e800b97-2c1b-43a8-b0f0-003f1543d2ba)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-compose)

## Details

Podman and Docker Compose are both command-line tools that use a specially formatted YAML file as input to assemble and then run single or multiple containers as applications.  These tools allow developers to develop, test, and then deliver to their users a single YAML file for their application and use only one command to start and stop it reliably.  This portability and reliability have made using the Compose specification hugely popular with users and developers, and it is increasingly becoming a requirement.

### Objectives

In this tutorial, you'll learn to:

   - Install and use both `podman-compose` and `docker-compose` with Podman
   - Verify they work with a simple `docker-compose.yaml` file

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - [Podman](https://docs.oracle.com/en/operating-systems/oracle-linux/podman/podman-InstallingPodmanandRelatedUtilities.html#podman-install) and cURL packages
    - Access to the Internet

