---
title: "Migrate Standalone Oracle Autonomous Linux Instances"
date: 2022-08-03
draft: false
summary: "Learn to use a migration script to migrate older standalone Oracle Autonomous Linux instances to integrate with and be managed by the OS Management service in Oracle CLoud Infrastructure."
tags: ["osms","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/8848ec22-81cd-46d5-aeab-dd2dae36118b)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/alx-linux-migrate)

## Details

Standalone Autonomous Linux instances are instances created with older Oracle Autonomous Linux images, typically from July 2021 and earlier.

These instances are referred to as standalone because, when created, they are not integrated by default with the OS Management service in Oracle Cloud Infrastructure.

An `alx-migrate` script has been created to migrate these standalone instances to be managed by the OS Management service. Oracle Autonomous Linux instances built with images from August 2021 onwards are by default integrated with the OS Management service.

After the script is installed, the migration can be performed, and the instance registered and then managed using the OS Management service. It then takes advantage of the additional autonomous capabilities provided by the service, such as monitoring processes and critical events, and automatic daily updating and patching.

> **Note:** The migration script can also be used with the Oracle Linux KVM Image, the Autonomous Linux version, with Unbreakable Enterprise Kernel. This lab uses an older Oracle Autonomous Linux image to create an instance suited for migration during the lab.

You can read more detailed information about prerequisites and using this migration script at this documentation link: [Migrating a Standalone Autonomous Linux Instance to the OS Management Service](https://docs.oracle.com/en-us/iaas/os-management/osms/alx-migrate.htm)

### Objectives

In this lab, you will learn to:

   - Create an Oracle Autonomous Linux instance using a 2021 custom image
   - Use the cloud console to determine a pre built Oracle Autonomous Linux 7 system to be a migration canditate
   - Verify instance plugins are enabled to support the migration process
   - Install the migration script on the instance
   - Run the migration script to integrate the instance with the OS Management service
   - Verify the successful migration


### Prerequisites

Specific Oracle Cloud IAM (Identity and Access Management) policies are needed to integrate OS Management service support with the migrated Oracle Autonomous Linux instance. During the migration the Oracle Cloud Agent and OS Management Service Agent plugins are stopped and restarted, policies must be in place to allow this.

The required cloud policies needed are already configured for the tenancy and compartment used for this lab.

You can read about the policies required for instances to be managed by the OS Management service at this link: [Required IAM Policies for OS Management integration](https://docs.oracle.com/en-us/iaas/os-management/osms/alx-getstarted.htm#alx-create-policies)


