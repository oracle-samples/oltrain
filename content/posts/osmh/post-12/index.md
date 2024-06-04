---
title: "Create Software Sources with Package Lists"
date: 2023-09-15
draft: false
summary: "Learn how to create Oracle OS Management Hub custom and versioned custom software sources for Oracle Linux from a reference package list."
tags: ["osmh","tutorial","osmh-admin"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/osmh-custom-swsrc-pkglist)

## Details

Custom software sources in OS Management Hub let you control the packages and modules available to your managed instances. OS Management Hub has flexible and powerful options for creating custom software sources. You can apply filters to limit the set of packages and modules or provide a reference package list from an existing Oracle Linux instance. Package dependencies can also be auto-resolved. You can create custom software sources using the Oracle Cloud Console, the OCI CLI, or programmatically with the OCI API/SDK. In this tutorial, you’ll learn how to take a reference package list from an Oracle Linux instance and use Oracle Cloud Console to create a custom or versioned custom software source in OS Management Hub.

### Objectives

In this tutorial, you will learn how to:

- Create Oracle OS Management Hub custom and versioned custom software sources for Oracle Linux from a reference package list.

### Prerequisites

- Access to your OCI tenancy
- OCI Privileges to read OS Management Hub managed instances and create software sources in OCI
- A reference Oracle Linux system
