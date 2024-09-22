---
title: "Running Auditd"
date: 2022-04-05
draft: false
summary: "Learn how to install, configure, and use the auditing daemon on Oracle Linux."
tags: ["ol","lab","tutorial","ol-monitor"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/3a72b337-d8c0-41b9-9193-e1bf50ad2ac9)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-auditd)

## Details

Auditd is a userspace system daemon running in the background, generating logs about activities performed on Oracle Linux.

### Objectives

In this tutorial, you'll learn to:

   - Install the audit packages
   - Manage the audit service
   - Create audit rules
   - Search the audit logs

### Prerequisites
- Minimum of two Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
   - A non-root user account with sudo access
