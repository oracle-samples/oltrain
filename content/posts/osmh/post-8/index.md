---
title: "Creating Lifecycle Environments"
date: 2023-10-04
draft: false
summary: "Learn to create a lifecycle environment in Oracle OS Management Hub."
tags: ["osmh", "video","osmh-dev"]
showDate: true
---

{{< youtube id="_Gq2TfYiEo8" title="Creating Lifecycle Environments in Oracle OS Management Hub" >}}

## Details

This video provides a step by step walk-through of creating a lifecycle environment in Oracle OS Management Hub. A lifecycle environment in Oracle OS Management Hub is a user-defined pipeline used to take versioned custom software sources from development and testing stages to production environments through a staged approach. Custom operating system software can be deployed along a title controlled set of lifecycle stages. Each stage has registered instances or systems that recieve the versioned custom software when it is promoted.

To manage content in the lifecycle environment, you create a versioned custom software source, which is a type of custom software source that's given a version and is immutable. Then you promote content by associating a versioned custom software source to a lifecycle stage. Only the instances assigned to that stage have access to the content in the versioned custom software source.

To learn how to create a custom versioned software source checkout the video selecting software sources for Oracle OS Management Hub and review the Creating Custom software source [documentation](https://docs.oracle.com/iaas/osmh/doc)

To create and setup a lifecycle environment in Oracle OS Management Hub, we will:

- Create a Lifecycle environment in the Oracle Cloud Infrastructure web console
- Define lifecycle stages for the lifecycle environment during creation
- View the Lifecycle Environment details page
- Add new instances using a stage-specific registration profile
- Attach existing, registered instances to lifecycle stages
