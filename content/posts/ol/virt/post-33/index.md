---
title: "Deploy HAProxy"
date: 2023-03-09
draft: false
summary: "Learn how to deploy and run HAProxy from a container using Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a9eb9ff9-b56d-4ddc-9283-b72467d78128)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-quay)

## Details

HAProxy is a well known, and widely used, open source solution delivering load balancing and proxy services for both HTTP (Layer 7) and TCP (Layer 4) which is achieved by spreading  incoming request across multiple servers.  For more details of the services that HAProxy _does_ and _does not_ provide please refer to the [upstream documentation](https://docs.haproxy.org).  HAProxy can be installed locally on [Oracle Linux](https://docs.oracle.com/en/operating-systems/oracle-linux/8/balancing/balancing-SettingUpLoadBalancingbyUsingHAProxy.html), or run as a container using Podman.  This lab describes how to use HAProxy with Podman.

> **Clarification:** This document follows the long established custom which suggests that the term _"HAProxy"_ is used to represent the product, whereas _"haproxy"_ is used to represent the executable.  Although many other sources use these forms interchangeably.

### Objectives

This lab shows how to:

  - Use HAProxy as a Podman-based container
  - Configure a simple deployment using three back-end servers
  - Confirm the deployment runs as expected

  > **Note:** The steps provided do not include how to configure HAProxy to use certificates.  Therefore its recommended for non-production purposes or an internal/air-gapped environment.

### Requirements

Four systems with Oracle Linux and Podman installed, whose responsibilities are divided like this:

   | Server Name | Role/Purpose                |
   |:------------|:----------------------------|
   | _ol-server_ | Hosts HAProxy load balancer |
   | _web01_, _web02_, _web03_ | Hosts the web application |

