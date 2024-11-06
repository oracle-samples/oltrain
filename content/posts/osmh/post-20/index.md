---
title: "Using the Policy Advisor"
date: 2023-08-15
draft: false
summary: " In this video, you will learn how to run the policy advisor setup in compartments that contain compute instances and/or management agent resources that will be managed by OS Management Hub."
tags: ["osmh","video","osmh-deploy"]
showDate: true
---

{{< youtube id="PypMjSfz9bQ" title="Using the Policy Advisor to enable Oracle OS Management Hub" >}}

## Details

Learn how to use the policy advisor tool in Oracle OS Management Hub to create groups and policies that enable the service to manage resources and users to manage the service in the Oracle Cloud Infrastructure web console. In this video, you will learn how to run the policy advisor setup in compartments that contain compute instances or management agent resources that will be managed by OS Management Hub.

The policy advisor can be found on the overview page of the OS Management Hub section in the OCI console. The policy advisor tool is compartment specific so it will need to be run in each compartment that will contain managed instances and resources. 

The advisor defines the necessary user groups (osmh-admins & osmh-operators), dynamic group(osmh-instances), and policies (osmh-policies) required to use OS Management Hub and Resource Discovery and Monitoring. The policy advisor creates two user groups, dynamic group, and policy with the required policy statements that enable users to administer or operate OS Management Hub and its resource discovery and monitoring features.
