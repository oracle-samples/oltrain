---
title: "Mirror a Yum Repository"
date: 2021-04-01
draft: false
summary: "Learn to mirror and share a Yum repository with local, offline, or distributed systems."
tags: ["ol","lab","tutorial","ol-package"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/b3779123-c17c-4f89-bb93-8c343d891825)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-yum-mirror)

## Details

The task of mirroring a yum repository holds multiple benefits. These include the following:

- Provide access to yum repositories for systems without access to a public network
- Improve software download times and reduce the bandwidth overhead of a large infrastructure
- Configure local network-based installation strategies
- Catering for a snapshot style update strategy where performing testing against a controlled software distribution environment

This tutorial shows how to mirror a yum repository for local, offline, or distributed systems access.

### Objectives

In this lab, you'll learn how to:

   - Prepare a system to host the repository mirror
   - Install and configure a web server
   - Download and create a local repository
   - Configure a system to access the repository mirror

### Prerequisites

  - Two Oracle Linux systems, one for the server and the other as a client
  - Storage with enough free space to contain the repository mirror

