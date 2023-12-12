---
title: "Managing Oracle Linux Module Streams and Profiles"
date: 2022-09-23
draft: false
summary: "Learn how to enable and install modules, select stream versions, and install profiles using the OS Management service."
tags: ["osms","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6abfafd9-749e-4b28-93ea-830b6046501d)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/ol-module-streams)

## Details

Oracle Linux AppStreams introduced the concept of modules, streams and profiles that allow for the management of different versions of software applications within a single OS release. From the Oracle Cloud Infrastructure console the OS Management service can manage instance modules and AppStreams, including viewing module information and updating modules, streams, and profiles. Similarly, from the command line, AppStreams on a single instance can also be installed and managed.

You can read more detailed information about module streams at this documentation link: [Managing Module Streams and Profiles](https://docs.oracle.com/en-us/iaas/os-management/osms/osms-manage-modules.htm)

## Objectives

In this lab, you will learn to:

   - Enable a module stream for PHP on an Oracle Linux Instance
   - Verify the stream on the instance with CLI
   - Inspect the available module streams and verify the packages installed for different profiles
   - Configure a stream profile and verify it is enabled
   - Monitor the work requests for managing streams with the OS Mangement service
   - Disable a module stream


### Prerequisites

Specific Oracle Cloud IAM (Identity and Access Management) policies are needed to support the OS Management service for Oracle Linux instances.

The required cloud policies needed are already configured for the tenancy and compartment used for this lab.

You can read about the policies required for instances to be managed by the OS Management service at this link: [Required IAM Policies for OS Management integration](https://docs.oracle.com/en-us/iaas/os-management/osms/alx-getstarted.htm#alx-create-policies)


