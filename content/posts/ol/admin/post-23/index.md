---
title: "Run cgroups v2"
date: 2022-03-22
draft: false
summary: "Learn how to enable and run cgropus v2 on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/14d89b6d-627b-4f1f-b859-4761e3ed352c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-cgroup-v2)

## Details

Control Groups (cgroups) is a Linux kernel feature for limiting, prioritizing, and allocating resources such as CPU time, memory, and network
bandwidth for running processes.

Thse guides walk you through limiting the CPU time for user processes using cgroups v2.

### Objectives

In this lab, you'll learn to:

   - Enable cgroups v2
   - Set a soft CPU limit for a user process
   - Set a hard CPU limit for a user process

### Prerequisites

  - A system with Oracle Linux 8 installed with the following configuration:
      - a non-root user with `sudo` permissions

