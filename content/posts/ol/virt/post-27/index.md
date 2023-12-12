---
title: "Build a DNF Repo Mirror"
date: 2022-03-10
draft: false
summary: "Learn how to use podman or docker to run a ULN or yum mirror service in a container."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/42ce804b-ce7c-4fc0-9baf-aaccc4d80495)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-reposync)

## Details

Oracle Linux 8 includes a fully functional **reposync** tool for DNF, that makes it easy to create a mirror of any yum repository. This facility can be extended to also mirror ULN channels for environments where the majority of your systems do not have direct access to the internet. By creating a yum mirror of the yum repositories and ULN channels that your organization uses, you can reduce network overhead and improve yum performance across your environment. Yum mirrors are also useful if you are configuring other services for your environment such as offline Ksplice.

While previous releases of Oracle Linux included a `uln-yum-mirror` package that could be used to perform mirroring services, this was not particularly efficient and was relatively complicated to set up.

A ULN or yum mirror service is a typical example of a service that is best run within a set of containers. By using either Docker or Podman, you can quickly and easily deploy a container that uses the `oraclelinux:8-slim` image to handle scheduled synchronization of the yum repositories or ULN channels that you use within your organization. You can also deploy a container that handles the provisioning of the mirrored repositories within a web service that client systems are able to access.

An opensource GitHub project provides the Dockerfiles, scripts and instructions to do set up this kind of service at [https://github.com/Djelibeybi/oraclelinux-reposync](https://github.com/Djelibeybi/oraclelinux-reposync).

### Objectives

In this lab, you'll learn to:

   - Install container-tools
   - Build a container with the required software
   - Create a mirror service using reposync within the container

### Prerequisites

  - A system with Oracle Linux 7 or Oracle Linux 8 installed and with access to the internet.
  - This tutorial assumes that you are using Oracle Linux 8, so package install commands use **dnf**, if you are using Oracle Linux 7, substitute these command instructions with **yum**.
  - In this tutorial, we use Podman and Buildah to handle the build and running of containers, but if you are using Oracle Linux 7, you can equally use Docker to perform these tasks.

