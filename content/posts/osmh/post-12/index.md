---
title: "Create Custom Software Sources"
date: 2023-09-15
draft: false
summary: "Learn how to create Oracle OS Management Hub custom and versioned custom software sources for Oracle Linux from a reference package list using the OCI CLI."
tags: ["osmh","tutorial","osmh-admin"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/osmh-custom-swsrc-cli)

## Details

Creating your own customized Oracle OS Management Hub software sources is powerful. Using the OCI console, you can apply filters to limit the set of packages and modules to just those you want and create a custom software source or versioned custom software source. Sometimes, using the filters to generate a lengthy set of packages at just the patch level you want is impractical. There is a faster and more streamlined way to create custom and versioned custom software sources using the OCI CLI. OS Management Hub integrates fully with the OCI CLI and the OCI API/SDK, so you can programmatically interact with the service. In this tutorial, you'll learn how to take a reference package list from an Oracle Linux instance and use the OCI CLI to create a custom or versioned custom software source in OS Management Hub.

### Objectives

In this tutorial, you will learn how to:

- Create Oracle OS Management Hub custom and versioned custom software sources for Oracle Linux from a reference package list using the OCI CLI

### Prerequisites

- Access to your OCI tenancy
- [OCI Privileges](https://docs.oracle.com/iaas/osmh/doc/getstarted.htm#required-iam-policies) to read OS Management Hub managed instances and create software sources in OCI
- [OCI API Signing Key](https://docs.oracle.com/iaas/Content/API/Concepts/apisigningkey.htm) is created and your ~/.oci/config is setup
- [OCI CLI v3.29.2](https://docs.oracle.com/iaas/Content/API/SDKDocs/cliinstall.htm#Quickstart) or newer installed (check with oci --version)
- A reference Oracle Linux 7, 8, or 9 system and its OCID (if managed by OS Management Hub)
- The OCID of your OCI tenancy
- Access to the internet
