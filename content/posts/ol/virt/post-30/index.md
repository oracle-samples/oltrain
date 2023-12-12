---
title: "Using Compose Files"
date: 2023-01-20
draft: false
summary: "Learn how to use Docker Compose functionality with Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/0e800b97-2c1b-43a8-b0f0-003f1543d2ba)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-compose)

## Details

Docker Compose is a command-line tool that uses a specially formatted YAML file as input to assemble and then run single, or multiple, containers as applications.  This allows developers to develop, test and then deliver to their users a single YAML file for their application, and use only one command to start, and stop, it reliably.  This portability and reliability has made Docker Compose not only hugely popular with both users and developers, but increasingly a requirement.

### Objectives

This lab shows how to install and use both `podman-compose` and `docker-compose` with Podman, and verify they work with a simple `docker-compose.yaml` file.

### Prerequisites

  - A client system with Oracle Linux installed
  - Podman installed (the 'container-tools' package)
  - Access to the Internet

