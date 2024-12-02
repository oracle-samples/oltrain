---
title: "Manipulate Files"
date: 2024-02-05
draft: true
summary: "Learn to use Oracle Linux Automation Engine to manipulate files and directories on an Oracle Linux instance."
tags: ["olam","lab","tutorial","olae"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/515f0a43-7478-48aa-88b8-daa2229b97c5)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olae-manipulate-files)

## Details

This tutorial shows how to create and delete files and directories on your remote hosts. 

### Objectives

In this lab, you'll learn to:

   - Create an empty file
   - Create a file with content
   - Create multiple files in a single task
   - Set file permissions
   - Create a directory
   - Remove files and directories

### Prerequisites

  - Install an Oracle Linux system with the following configuration:
      - a non-root user with `sudo` permissions
      - ssh keypair for the non-root user
      - the ability to ssh from one host (control-node) to the other (host) using passwordless ssh login
