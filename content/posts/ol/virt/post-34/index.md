---
title: "Deploy Quay in HA"
date: 2023-03-31
draft: false
summary: "Learn how to deploy a High Availabilty Project Quay Registry Configuration on Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a63c2548-c459-457f-b3d1-123c99d90d89)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-ha-quay)

## Details

Project Quay is an open-source repository used to store and manage artefacts such as containers for use on cloud native platforms.  Project Quay also offers additional functionality such as (in no particular order):

  - Registry - High availability
  - Security - Vulnerability scanning, Logging & Auditing, Notifications & Alerts
  - Access Control - Role-based access control (RBAC)
  - Integration - OAuth support
  - Build Automation - Git/GitHub/GitLab integration

It can be deployed on either a Kubernetes cluster using an Operator, or as a standalone container or high availability cluster on Podman.

### Objectives

This lab demonstrates how to:

 - Access a 3-node Project Quay deployment
 - Verify basic Project Quay functionality works
 - Use the HAProxy Console to monitor Project Quay nodes

  > **Note:** The steps provided do not include how to configure the registry using certificates.  Therefore, configuring Project Quay in this specific way is recommended for non-production purposes or an internal/air-gapped environment only.

### Requirements

Four systems with Oracle Linux, Podman, Redis, PostgreSQL, HAProxy and Project Quay installed, whose responsibilities are apportioned like this:

   | Server Name | Role/Purpose                                                        |
   | ----------- | ------------------------------------------------------------------- |
   | _ol-server_ | Hosts the HAProxy load balancer and the Postgres database           |
   | _quay01_, _quay02_, _quay03_ | Hosts the Project Quay and Redis servers |

In addition the requisite security rules to allow TCP and/or HTTP traffic to permit the above to work must be configured correctly.<br>

> **Note:** This lab builds upon these two previous labs, which provide details explaining how to install and configure both HAProxy and Project Quay, respectively:
>
>   - [Learn to install Project Quay on Podman](https://luna.oracle.com/lab/e3f488a9-20a8-49d8-ae08-818f8730568c)
>   - [Deploy HAProxy using Podman](https://luna.oracle.com/lab/a9eb9ff9-b56d-4ddc-9283-b72467d78128)
>
