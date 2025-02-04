---
title: "Use Pasta Networking"
date: 2025-02-04
draft: false
summary: "Learn how to use Pasta Networking with Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6cc1f2f1-5a2b-44cb-8662-b89aec478449)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-pasta-networking)

## Details

[Oracle Linux 9 Update 5](https://docs.oracle.com/en/operating-systems/oracle-linux/9/relnotes9.5/ol9-features-Containers.html#OLRNT-ol9.5-features-Containers_podman_5.2) changed the default tool for rootless container networking from `slirp4netns` to `pasta`. So what is [Podman `pasta` networking](https://passt.top/passt/about/)? Pasta is an acronym for "Pack A Subtle Tap Abstraction".

Pasta uses the `passt` network driver, introduced in [Oracle Linux 9 Update 1](https://docs.oracle.com/en/operating-systems/oracle-linux/9/relnotes9.2/ol9-NewFeaturesandChanges.html#OLRNT-ol92-features-virtualization_passt_package_introduced), to allow rootless containers to create a network namespace and forward network traffic to the namespace. Pasta networking uses the `passt` driver as a translation layer between a Layer-2 network interface and Layer-4 socket traffic using TCP, UDP, and ICMP echo on the host. Pasta networking does not require elevated privileges (root), which allows Podman to run rootless containers.

Podman pasta networking delivers these benefits:

- Seamlessly integrated with Podman v4.1 and higher and is the default from Podman 5.3 onwards.
- Improved network performance for rootless containers, especially compared to alternatives such as `slirp4netns`.
- Designed to work with rootless containers, allowing users to run containers without requiring elevated privileges and enhancing system security.
- Uses the host's IP address instead of the `slirp4netns` method, which uses a predefined container IP address.
- Uses a network interface name from the host instead of the `slirp4netns` default of `tap0`.

### Objectives

In this tutorial, you'll learn to:

- Define and use `pasta` networks with Podman
- Verify a container is using `pasta` networking

### Prerequisites

- Two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
  - A non-root user account with sudo access
  - The latest Oracle Linux Release
  - [Podman](https://docs.oracle.com/en/operating-systems/oracle-linux/podman/podman-InstallingPodmanandRelatedUtilities.html#podman-install) and cURL packages
  - Access to the Internet
