---
title: "Use Lifecycle Environments"
date: 2025-03-31
draft: false
summary: "Learn to create and use lifecycle environments in Oracle OS Management Hub."
tags: ["osmh","lab","tutorial","osmh-dev"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/2c4e8bb8-d2d8-4a48-8752-cc44ad9668f4)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/osmh-lifecycle)

## Details

Learn to create and use lifecycle environments to promote versioned custom software sources through lifecycle stages in Oracle OS Management Hub.

### Objectives

In this tutorial, you'll learn how to:

  - Create a lifecycle environment and define three lifecycle stages
  - Register existing OCI compute instances to lifecycle stages using profiles
  - Create a versioned custom software source using a package list
  - Promote the versioned custom software source to the first stage in the lifecycle environment
  - Promote the versioned custom software source through the remaining stages in the lifecycle environment

### Prerequisites

Access to an Oracle Cloud Infrastructure tenancy with:

  - An administrative user group, a dynamic group identifying instance resources, and the IAM policies that enable OS Management Hub.
  - Oracle Linux compute instances.
  - The following vendor software sources:
     - ol8_baseos_latest-x86_64
     - ol8_appstream-x86_64
     - ol8_addons-x86_64
     - ol8_uekr6-x86_64
  - Virtual Cloud Network (VCN) or configured network access that supports OS Management Hub.
