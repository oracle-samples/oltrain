---
title: "Virtualization"
date: 2020-08-03
weight: 02
draft: false
description: "Virtualization"
summary: "This page focuses on Kernel-based Virtual Machine (KVM), Containers, Podman, chroot, and Kubernetes. It covers lessons on installation, management, creation and other aspects related to using virtualization on Oracle Linux."
tags: [ "kvm","cockpit","containers","podman"]
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
aliases:
- /OL/virt/virt.html
series: ["Oracle Linux"]
series_order: 11
---

{{< figure src="/img/ol/virt/OL-virt-kvm.png" alt="virt-kvm" >}}

## KVM

{{< card2 limit=30 tag="/tags/ol-kvm" >}}

{{< figure src="/img/quiz1.png" alt="ol-virt-kvm-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:CPXRPS1" target="_blank" >}}
Take the quiz
{{< /button >}}

{{< figure src="img/ol/virt/OL-virt-containers.png" alt="Containers" >}}

## Podman

{{< card2 limit=30 tag="/tags/ol-podman" >}}


### Containers - A High-Level Overview

- {{< youtube V9sOZHfuvVM >}}

### Are Containers Virtual Machines?

- {{< youtube AvNDTpmHOMk >}}

### Install Podman, Buildah, and Skopeo on Oracle Linux

- {{< youtube L9Arzr88p0M >}}

### Search Container Registries with Podman on Oracle Linux

- {{< youtube id="p2FxmHbPFqM" title="Search Container Registries with Podman on Oracle Linux" >}}

### Pull Images with Podman on Oracle Linux

- {{< youtube id="DFtZYIOPcuU" title="Pull Images with Podman on Oracle Linux" >}}

### Run Containers with Podman on Oracle Linux

- {{< youtube id="-eRlcn3l_Sk" title="Run Containers with Podman on Oracle Linux" >}}

### Using Public Registries with Podman on Oracle Linux

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

### [Run Containers with Podman on Oracle Linux](https://luna.oracle.com/lab/2f0beeef-bc10-4e54-a042-ce31db0e9765)

This lab will guide you through running and managing containers with Podman on Oracle Linux. It shows how to search and pull images from container registries and create containers with them.  

You will start, stop and attach to containers, and execute commands in running containers. Viewing container logs, and removing containers and images are all covered in this lab.

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

### [Deploy Keycloak using Podman on Oracle Linux](https://luna.oracle.com/lab/752793ff-9f74-4bb0-b848-90c5bcae4388)

Learn to deploy Keycloak for providing authentication to applications and secure services using OAuth and SAML.

Keycloak provides single sign-on functionality for web applications and RESTFUL web services. A primary goal of Keycloak is to provide security features that developers can easily use to secure applications and services within their organizations, for example Single-Sign-On authentication. Keycloak can also be integrated with existing LDAP and Active Directory servers.

Keycloak is based on standard protocols and provides support for User Federation, OpenID Connect, OAuth 2.0 and SAML and many more. Keycloak provides both administrators, and users, with management consoles. Users can update their passwords, profile details and setup two-factor authentication via the Account Management Console. Likewise administrators can use the Admin Console to manage all aspects of Keycloak's functionality, it's authorization policies, applications and manage users (including user's permissions and sessions).

---

### [Deploy HAProxy using Podman](https://luna.oracle.com/lab/a9eb9ff9-b56d-4ddc-9283-b72467d78128)

Learn to setup and use a HAProxy container on Podman.

HAProxy is a well known, and widely used, open source solution delivering load balancing and proxy services for both HTTP (Layer 7) and TCP (Layer 4) which is achieved by spreading incoming request across multiple servers. For more details of the services that HAProxy does and does not provide please refer to the [upstream documentation](https://docs.haproxy.org/). HAProxy can be installed locally on Oracle Linux , or run as a container using Podman. This lab describes how to use HAProxy with Podman.

---

### [Deploy a High Availability Project Quay using Podman](https://luna.oracle.com/lab/a63c2548-c459-457f-b3d1-123c99d90d89)

Learn to setup and use a high availability deployment of Project Quay Registry on Podman.

---

### [Install kind Using Rootless Podman on Oracle Linux](https://luna.oracle.com/lab/30610e81-95e7-4c54-85bc-efcb5e757e04)

Learn how to install _kind_ using rootless Podman on Oracle Linux.

[kind](https://kind.sigs.k8s.io/) is an open source tool for running a locally hosted Kubernetes cluster using Podman containers as the cluster nodes.  It is specifically designed to provide both Developers and DevOps administrators to quickly create a Kubernetes cluster on a single machine without requiring the complicated and lengthy process of bootstrapping and then configuring the cluster, etc.  Instead kind maintains all the components for both control plane and worker nodes.

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
