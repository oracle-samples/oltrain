---
title: "Install Project Quay"
date: 2023-02-15
draft: false
summary: "Learn to run and configure the Project Quay container image registry on Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/e3f488a9-20a8-49d8-ae08-818f8730568c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-quay)

## Details

Project Quay is an open-source repository that stores and manages artifacts such as containers for use on cloud-native platforms. Project Quay also offers additional functionality such as (in no particular order):

   - Registry - High availability
   - Security - Vulnerability scanning, Logging & Auditing, Notifications & Alerts
   - Access Control - Role-based access control (RBAC) 
   - Integration - OAuth support
   - Build Automation - Git/GitHub/GitLab integration 

It can be deployed on a Kubernetes cluster using an Operator or as a standalone container or high-availability cluster on Podman.  

### Objectives

In this tutorial, you'll learn how to:

   - Install and run Project Quay using Podman
   - Verify basic Quay functionality is working

   > **Note:** The steps provided do not include configuring the registry using certificates. Therefore, it's recommended for non-production purposes or an internal/air-gapped environment.

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
   - A non-root user account with sudo access
   - Podman and cURL packages
   - Access to the Internet
