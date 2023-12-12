---
title: "Install Project Quay"
date: 2023-02-15
draft: false
summary: "Learn to setup and use the Project Quay Registry on Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/e3f488a9-20a8-49d8-ae08-818f8730568c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-quay)

## Details

Project Quay is an open-source repository used to store and manage artifacts such as containers for use on cloud native platforms.  Project Quay also offers additional functionality such as (in no particular order):

- Registry - High availability
- Security - Vulnerability scanning, Logging & Auditing, Notifications & Alerts
- Access Control - Role-based access control (RBAC)
- Integration - OAuth support
- Build Automation - Git/GitHub/GitLab integration

It can be deployed on either a Kubernetes cluster using an Operator, or as a standalone container or high availability cluster on Podman.

### Objectives

These guides show how to install and run Project Quay on Podman and then confirm it is working.  The main steps described are outlined below:

  - Install Project Quay on Podman
  - Verify basic Quay functionality works

  > **Note:** The steps provided do not include how to configure the registry using certificates.  Therefore its recommended for non-production purposes or an internal/air-gapped environment.

### Requirements

  - A system with Oracle Linux installed
  - Podman installed (the 'container-tools' package)
  - Access to the Internet

