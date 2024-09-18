---
title: "Maintain Security with DNF"
date: 2023-09-12
draft: true
summary: "Learn to use DNF for security package maintenance on Oracle Linux."
tags: ["ol","lab","tutorial","ol-package"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/b48151dc-20d9-4c52-b868-840978f4a514)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-dnf-security)

## Details

The following guides provide practical examples of using the Dandified YUM (DNF) package manager on Oracle Linux to apply maintenance and security updates. This tutorial is targeted at users of Oracle Linux 8 or later.

DNF downloads packages from enabled repositories for install and update actions. It performs automatic dependency resolution for packages and installs all packages needed to fulfill dependency requirements. DNF also includes integrated options for managing security and errata updates available for packages installed in Oracle Linux.

A security patch is an update to fix a specific vulnerability incorporating changes in source code. These security patches usually apply to particular software components.

A bug fix is the elimination of known software errors.

CVE is short for Common Vulnerabilities and Exposures. It is a list of publicly disclosed computer security flaws. A CVE refers to a security flaw where a CVE Numbering Authority (CNA) assigns a CVE ID number. Security advisories usually refer to at least one CVE ID, with a priority ranging from negligible through low, medium, high to critical.

Enterprise Linux denotes these specific updates as:

  - `ELSA` : Enterprise Linux Security Advisory patches
  - `ELBA` : Enterprise Linux Bug Fix Advisory patches
  - `ELEA` : Enterprise Linux Enhancement Advisory patches

### Objectives

In this lab, you'll learn:

  - The meaning of CVEs, ELSAs, and Bug Fixes
  - To use DNF for installing security updates
  - That package updates are cumulative and have dependencies
  - To clean up old packages

### What Do You Need?

  - An Oracle Linux system.

