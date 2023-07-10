---
title: "Virtualization"
date: 2020-08-03
draft: false
description: "Virtualization"
summary: "This page focuses on Kernel-based Virtual Machine (KVM), Containers, Podman, chroot, and Kubernetes. It covers lessons on installation, management, creation and other aspects related to using virtualization on Oracle Linux."
tags: [ "Virtualization", "KVM", "Network Bridge", "Cockpit" ]
slug: "virt"
showRecent: false
showDate: false
showLikes: false
showViews: false
showEdit: false
showReadingTime: false
showAuthor: false
showDateUpdated : false
sharingLinks : false
cascade:
  showDate: false
  showAuthor: false
  invertPagination: true
---

{{< figure src="/img/ol/virt/OL-virt-kvm.png" alt="virt-kvm" >}}

## KVM Videos

### Enabling KVM on Oracle Linux

- {{< youtube ALtnopSysY4 >}}

### Setup Cockpit Web console to Manage KVM on Oracle Linux

- {{< youtube -Z3AwP2HPa4 >}}

### Using Cockpit to Create KVM VMs on Oracle Linux

- {{< youtube daHQeCY13s8 >}}

### SSH into a NAT based KVM VM on Oracle Linux

- {{< youtube 2MEqDxOeuDw >}}

### Create a Network Bridge for KVM on Oracle Linux

- {{< youtube OAfIb7gtang >}}

### Using a Network Bridge with KVM VMs on Oracle Linux

- {{< youtube CXBTBxFoSKI >}}

### Switch a KVM VM from NAT to Bridged on Oracle Linux

- {{< youtube hMstMTqzP_Q >}}

### Convert and Deploy a VirtualBox VM to KVM on Oracle Linux

- {{< youtube 7gZLiTa3150 >}}

### Add a disk to an existing KVM VM on Oracle Linux

- {{< youtube B3h_DWOMwrk >}}

## KVM Labs

### [Create VMs with KVM on Oracle Linux](https://luna.oracle.com/lab/1671b073-895c-4800-bd60-cfe1f445074c)

Learn how to deploy KVM on Oracle Linux to create and manage virtual machines.

Kernel-based Virtual Machine (KVM) is an open-source type-1 (bare-metal) hypervisor. This functionality permits a host system, such as Oracle Linux 8, to host multiple virtual machines (VMs) or guests when running on supported hardware.

This lab will deploy Oracle Linux Kernel Virtualization Manager (KVM) to create a virtual machine.

[![](../../common/images/createvmkvm_lab.png)](https://luna.oracle.com/lab/1671b073-895c-4800-bd60-cfe1f445074c)

{{< figure src="/img/quiz1.png" alt="ol-virt-kvm-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:CPXRPS1" target="_blank" >}}
Take the quiz
{{< /button >}}

---

{{< figure src="img/ol/virt/OL-virt-containers.png" alt="Containers" >}}

## Container Videos

### Containers - A High-Level Overview

- {{< youtube V9sOZHfuvVM >}}

### Are Containers Virtual Machines?

- {{< youtube AvNDTpmHOMk >}}

### Install Podman, Buildah, and Skopeo on Oracle Linux

- {{< youtube L9Arzr88p0M >}}

### Pulling an Image using Podman on Oracle Linux

- {{< youtube QmZE-lFNzk4 >}}

### Using Public registries with Podman on Oracle Linux

- {{< youtube q57hNilpakk >}}

### Create a Local Registry with Podman on Oracle Linux

- {{< youtube 8wVmR_5YyCk >}}

### Running a Container using Podman on Oracle Linux

- {{< youtube PXeKEIdaTBs >}}

### Introduction to Image Layers with Podman on Oracle Linux

- {{< youtube i9KKMM0RiDI >}}

### Using Bind Mounts with Podman Containers on Oracle Linux

- {{< youtube Kw5vdNRRaZc >}}

### Using Volumes for Podman Container Storage on Oracle Linux

- {{< youtube qIjTMOfGa_Y >}}

### Using a Dockerfile with Podman on Oracle Linux

- {{< youtube AkvluNPzGSY >}}

### Using chroot on Oracle Linux

- {{< youtube dxzwxvn621w >}}

## Container Labs

### [Get started with Podman](https://luna.oracle.com/lab/4fa11b26-6c31-4595-ac00-b6c6af97f417)

Introduction to using Podman on Oracle Linux.  This lab gets you started using Podman on Oracle Linux 8 or later. You will install Podman, pull an image from a repository, and use the image to run a container.

---

### [Use storage with Podman containers](https://luna.oracle.com/lab/0dde3b49-0b91-423e-a126-5e718e05ca64)

Introduction to container storage on Oracle Linux.  This lab shows how to use different container storage types to access the host filesystem or persist files. This tutorial is targeted at users of Oracle Linux 8 or later.

---

### [Use a Container to Create a DNF or ULN Repo Mirror](https://luna.oracle.com/lab/42ce804b-ce7c-4fc0-9baf-aaccc4d80495)

This lab will guide you through creating a container that syncs content and layout from both yum.oracle.com or Oracle ULN, while mirroring the structure of yum.oracle.com.

---

### [Mount an NFS Share Using a Rootful Podman Volume](https://luna.oracle.com/lab/556e1401-568f-447e-8c0b-c94a86b1114f)

Learn how to use an NFS share as a volume for remote and persistent storage within a Podman container.

A Network File System or NFS is a distributed file system protocol originally developed by Sun Microsystems in 1984. NFS allows a user on a client computer to access files over the network, similar to how they access local storage.

When working with Podman containers, the need may arise to access files on an NFS share, which you accomplish using a Podman volume. Volumes are the preferred means to persist data generated and used by the containers. Podman completely manages volumes and differs from bind mounts as they are independent of the host machine's directory structure and OS.

This lab will show how to use Podman volumes to mount and access a remote NFS share.

---

### [Install Podman Desktop](https://luna.oracle.com/lab/55225d03-4fdb-42dd-bb3c-0382cb918963)

Learn to setup and use Podman Desktop.

Podman Desktop is a Graphical User Interface (GUI) for the Podman CLI, providing an easy way to interact with the Podman engine. Besides making it easy to confirm the status of the Podman engine itself, it also provides an easy way to review and interact with any containers deployed, images stored, and Podman pods and volumes that are present on the machine. On the other hand, note that it does not provide any extra functionality that is not available from the command-line.

---

### [Using Compose Files with Podman](https://luna.oracle.com/lab/0e800b97-2c1b-43a8-b0f0-003f1543d2ba)

Learn to setup and use Docker Compose files with Podman. 

Docker Compose is a command-line tool that uses a specially formatted YAML file as input to assemble and then run single, or multiple, containers as applications. This allows developers to develop, test and then deliver to their users a single YAML file for their application, and use only one command to start, and stop, it reliably. This portability and reliability has made Docker Compose not only hugely popular with both users and developers, but increasingly a requirement.

---

### [Learn to Install Project Quay on Podman](https://luna.oracle.com/lab/e3f488a9-20a8-49d8-ae08-818f8730568c)

Learn to setup and use the Project Quay Registry on Podman.

Project Quay is an open-source repository used to store and manage artifacts such as containers for use on cloud native platforms. Project Quay also offers additional functionality such as (in no particular order):

- Registry - High availability
- Security - Vulnerability scanning, Logging & Auditing, Notifications & Alerts
- Access Control - Role-based access control (RBAC)
- Integration - OAuth support
- Build Automation - Git/GitHub/GitLab integration

It can be deployed on either a Kubernetes cluster using an Operator, or as a standalone container or high availability cluster on Podman

---

### [Deploy HAProxy using Podman](https://luna.oracle.com/lab/a9eb9ff9-b56d-4ddc-9283-b72467d78128)

Learn to setup and use a HAProxy container on Podman.

HAProxy is a well known, and widely used, open source solution delivering load balancing and proxy services for both HTTP (Layer 7) and TCP (Layer 4) which is achieved by spreading incoming request across multiple servers. For more details of the services that HAProxy does and does not provide please refer to the [upstream documentation] (https://docs.haproxy.org/#xd_co_f=NjUzNDIzODAtMTcwNy00YzFlLTgxMDItNTM2YjIwZjBkMmQ0~). HAProxy can be installed locally on Oracle Linux , or run as a container using Podman. This lab describes how to use HAProxy with Podman.

---

### [Deploy a High Availability Project Quay using Podman](https://luna.oracle.com/lab/a63c2548-c459-457f-b3d1-123c99d90d89)

Learn to setup and use a high availability deployment of Project Quay Registry on Podman.

---

## Container Tutorials

### [Building multi-platform container images using Podman on Oracle Linux](https://docs.oracle.com/en/learn/oracle-linux-platform-images/index.html)

This tutorial shows the creation of a multi-platform container image using Podman on Oracle Linux 8 or later.

---

{{< figure src="/img/quiz1.png" alt="ol-virt-containers-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:CS8UESN" target="_blank" >}}
Take the quiz
{{< /button >}}
