---
title: "un Control Group Version 2"
date: 2022-03-22
draft: false
summary: "Learn how to use control group version 2 on Oracle Linux to limit the CPU time for user slices."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/14d89b6d-627b-4f1f-b859-4761e3ed352c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-cgroup-v2)

## Details

Control Group (cgroup) is a Linux kernel feature for limiting, prioritizing, and allocating resources such as CPU time, memory, and network
bandwidth for running processes.

This tutorial guides you through limiting the CPU time for user processes using cgroup v2.

### Objectives

In this tutorial, you will learn how to:

   - Enable control group version 2
   - Set a soft CPU limit for a user process
   - Set a hard CPU limit for a user process

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet
