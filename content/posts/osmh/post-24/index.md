---
title: "Rerun a Failed Job"
date: 2025-03-19
draft: false
summary: "Learn to rerun a failed job in Oracle OS Management Hub."
tags: ["osmh","tutorial","osmh-admin"]
showDate: true
---

## Links

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/osmh-rerun)

## Details

If a job fails, you can rerun the failed job instead of manually creating a new job to retry the failed action. You can rerun a failed job immediately or schedule it to run at a future date and time. Let’s review a failed job, examine the error logs, address the issue, and then rerun the failed job.

### Objectives

In this tutorial, you will learn how to:

- Run an install package job
- View Job statuses
- Examine error logs
- View an instance’s attached software sources
- Attach vendor software sources
- Rerun a failed job

### Prerequisites

- An administrative user group, a dynamic group identifying instance resources, and the IAM policies that enable OS Management Hub.
- Oracle Linux compute instance running Oracle Linux 8 and the following software sources:
  - ol8_baseos_latest-x86_64
  - ol8_addons-x86_64
  - ol8_appstream-x86_64
- Virtual Cloud Network (VCN) or configured network access that supports OS Management Hub.
