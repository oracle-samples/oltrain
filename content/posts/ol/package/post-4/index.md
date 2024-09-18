---
title: "Running DNF"
date: 2021-05-10
draft: false
summary: "Learn how to use DNF to manage packages and modules and apply security fixes on Oracle Linux."
tags: ["ol","lab","tutorial","ol-package"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/609f19ec-b142-4fa9-81d1-ab6d1e97478c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-dnf)

## Details

Oracle Linux provides the `dnf` utility, based on Dandified Yum (DNF), as the client software for installing and managing system packages. These packages can come from the Unbreakable Linux Network (ULN) or an Oracle Linux yum server. Software packages are installed on a system using standard dnf commands and depend on the system having enabled the appropriate ULN channel subscriptions or yum repositories. While installing or upgrading packages, `dnf` automatically handles package dependencies and requirements.

DNF significantly improves functionality and performance and brings many new features, including modular content and a more stable and documented API, compared to the traditional' yum' command.

### Objectives

In this tutorial, you'll learn how to:

   - Work with DNF repositories
   - Manage packages and modules
   - Install security updates
   - Leverage package groups
   - Use the DNF history feature
   - Automate patch upgrades

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet