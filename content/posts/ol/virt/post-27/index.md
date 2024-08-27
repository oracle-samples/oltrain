---
title: "Build a DNF Repo Mirror"
date: 2022-03-10
draft: false
summary: "Learn to use reposync in a container to create a DNF or ULN mirror service."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/42ce804b-ce7c-4fc0-9baf-aaccc4d80495)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-reposync)

## Details

Oracle Linux includes a fully functional **reposync** tool for DNF, making creating a mirror of any yum repository easy. We can also extend this facility to mirror ULN channels for environments where the majority of your systems do not have direct access to the internet. By creating a yum mirror of your organization's yum repositories and ULN channels, you can reduce network overhead and improve yum performance across your environment. Yum mirrors are also useful if you are configuring other services for your environment, such as offline Ksplice.

While previous releases of Oracle Linux included a `uln-yum-mirror` package that you could use to perform mirroring services, this was not particularly efficient and was relatively complicated to set up.

A ULN or yum mirror service is a typical example of a service that is best run within a set of containers. Using Podman, you can quickly and easily deploy a container that uses the Oracle Linux *slim* image to handle scheduled synchronization of the yum repositories or ULN channels that you use within your organization. You can also deploy a container that handles the provisioning of the mirrored repositories within a web service that client systems are able to access.

An opensource GitHub project provides the Dockerfiles, scripts, and instructions to set up this kind of service at [https://github.com/Djelibeybi/oraclelinux-reposync](https://github.com/Djelibeybi/oraclelinux-reposync).

### Objectives

In this tutorial, you'll learn to:

   - Install container-tools
   - Build a container with the required software
   - Create a mirror service using reposync within the container

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet

