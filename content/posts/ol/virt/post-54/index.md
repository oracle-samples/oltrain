---
title: "Use Quadlet with Systemd"
date: 2025-04-01
draft: false
summary: "Learn to run a rootless containers using Podman under systemd with Quadlet on Oracle Linux."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/014d85f3-f57c-4730-85a9-165f26531dd6)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-quadlet)

## Details

Quadlet provides a way to run containers under systemd within Oracle Linux. You define the container to run under a `[Container]` section in a familiar format to the standard Podman command line syntax and leverage all the benefits of the `[Unit]` and `[Service]` options of systemd. The advantage to using systemd to run your containers is that systemd is integrated into the operating system, so you can have containers that start when the system starts or set the order and dependency between a multi-container configuration.

Quadlet replaces an older method Podman used to integrate with systemd. That method consists of creating a container, generating a service file, moving the service file, and then enabling the service. In many cases, users would spend time writing these steps into Bash scripts and then have to maintain those scripts and the generated files. Depending on a user's perspective, Quadlet simplifies this task.

### Objectives

In this tutorial, you'll learn to:

- Create a *.container* file
- Start the new container service
- Test the container
- Update the container

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account with sudo access
  - [Podman](https://docs.oracle.com/en/operating-systems/oracle-linux/podman/podman-InstallingPodmanandRelatedUtilities.html#podman-install) and cURL packages
  - Cgroup v2
  - Access to the Internet
