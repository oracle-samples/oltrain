---
title: "Welcome to Oracle Cloud Native Environment Track"
date: 2020-08-03
draft: false
description: "Welcome to Oracle Cloud Native Environment Track"
summary: "This track contains videos to facilitate your usage of the technologies, software and tools used by Oracle to develop microservices-based applications that can be deployed in environments that support open standards and specifications.  Information and videos presented here cover Microservices technologies which are components of the Oracle Cloud Native Environment General Availability announcement, as well as additional technologies to help you expand your learning of microservices."
tags: ["OCNE", "Oracle Cloud Native Environment", "Kubernetes", "Istio" ]
slug: "ocne"
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
- /OCNE/ocne.html
---

{{< figure src="/img/ocne/OCNE-banner.jpg" alt="Oracle Cloud Native Environment Track" >}}

---

{{< lead >}} Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud-native applications.

Oracle Cloud Native Environment is a curated set of open source projects that are based on open standards, specifications and APIs defined by the Open Container Initiative (OCI) and Cloud Native Computing Foundation (CNCF) that can be easily deployed, have been tested for interoperability and for which enterprise-grade support is offered.

Oracle Cloud Native Environment delivers a simplified framework for installations, updates, upgrades and configuration of key features for orchestrating microservices. {{< /lead >}}

---

{{< figure src="/img/ocne/OCNE-environ-section.png" alt="Oracle Cloud Native Environment Installation section banner" >}}

## Environment Installation

### Installation Labs

Each lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment.

#### [Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/d18fe294-efb5-4498-9e7b-d5cc724d8619)

Learn how to install and configure Oracle Cloud Native Environment on Oracle Linux.

Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications. The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers. CRI-O manages the container runtime for a Kubernetes cluster. The runtime may be either runC or Kata Containers.

---

#### [Use Gluster with Oracle Cloud Native Environment](https://luna.oracle.com/lab/5455954d-142c-4801-9f34-5946ad19573d)

Learn how to set up and use Gluster with Oracle Cloud Native Environment.

The Gluster Container Storage Interface module can be used to set up statically or dynamically provisioned persistent storage for Kubernetes applications using Gluster Storage for Oracle Linux in Oracle Cloud Native Environment.  In this example, we will create an integrated system where Kubernetes worker nodes provide persistent storage using Gluster on Oracle Cloud Native Environment.

---

#### [Run a Compact Oracle Cloud Native Environment](https://luna.oracle.com/lab/c1bf32f7-7809-4355-bf83-d3f46797dd02)

Learn how to install and configure a compact deployment of Oracle Cloud Native Environment on Oracle Linux.

The 1.5 release of Oracle Cloud Native Environment introduced the compact deployment, allowing non-system Kubernetes workloads to run on control plane nodes. When setting --compact to true, the Platform API Server does not taint the control plane node(s). This setting allows non-system Kubernetes workloads to be scheduled and run on control plane nodes.

---

#### [Use OCI Cloud Controller Manager on Oracle Cloud Native Environment](https://luna.oracle.com/lab/5571f277-3eb9-435f-b3b3-fe421fb9747e)

Learn how to enable the Load balancer Service type in Oracle Cloud Native Environment on Oracle Cloud Infrastructure.

The Kubernetes LoadBalancer Service exposes the Deployment externally using a cloud provider's load balancer. The dependent NodePort and ClusterIP Services, to which the external load balancer routes, are automatically created.

This tutorial shows how to deploy the Oracle Cloud Infrastructure Cloud Controller Manager module (OCI-CCM module) within Oracle Cloud Native Environment to handle requests for an external LoadBalancer Service type. The Oracle Cloud Infrastructure Cloud Controller Manager module uses the open source oci-cloud-controller-manager project, which is a Kubernetes Cloud Controller Manager implementation (or out-of-tree cloud-provider) for Oracle Cloud Infrastructure (OCI).

---

#### [Deploy an External Load Balancer with Oracle Cloud Native Environment](https://luna.oracle.com/lab/be8d99fc-44c3-4062-a3c3-95e982243ccf)

Learn how to deploy a Highly Available Oracle Cloud Native Environment using the Oracle Cloud Infrastructure Load Balancer.

Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications. The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers. CRI-O manages the container runtime for a Kubernetes cluster. The runtime may be either runC or Kata Containers.

---

#### [Deploy Internal Load Balancer with Oracle Cloud Native Environment](https://luna.oracle.com/lab/15c6f5a7-9fec-4946-bb42-92dd41310fdf)

Learn how to deploy a Highly Available Oracle Cloud Native Environment using the Internal Load Balancer.

Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications. The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers. CRI-O manages the container runtime for a Kubernetes cluster. The runtime may be either runC or Kata Containers.

---

#### [Use MetalLB with Oracle Cloud Native Environment](https://luna.oracle.com/lab/d931637d-4e6b-4a46-ba17-810a942c4309)

Learn how to install and configure MetalLB together with Oracle Cloud Native Environment on Oracle Linux.

Network load balancers provide a method of externally exposing Kubernetes applications. A Kubernetes LoadBalancer service is used to create a network load balancer that provides and exposes an external IP address that can be used to connect to an application from outside the cluster.

MetalLB is a network load balancer for Kubernetes applications deployed on Oracle Cloud Native Environment running on bare metal hosts. MetalLB allows you to use Kubernetes LoadBalancer services, which traditionally make use of a cloud provider network load balancer, in a bare metal environment.

---

#### [Scale a Kubernetes Cluster on Oracle Cloud Native Environment](https://luna.oracle.com/lab/6c9e4d88-27e7-43bd-9366-0693fb8e4d3a)

Learn how to scale a Kubernetes Cluster on Oracle Cloud Native Environment.

This tutorial demonstrates how to scale an existing Kubernetes cluster in Oracle Cloud Native Environment.

To scale up a Kubernetes cluster means adding nodes, likewise scale down occurs by removing nodes. Nodes can be either control plane or worker nodes. Oracle recommends against scaling the cluster up and down at the same time. Instead perform a scale up, then scale down, in two separate commands.

This tutorial uses an existing Highly Available Kubernetes cluster running on Oracle Cloud Native Environment, and has three modules deployed:

- Kubernetes (kubernetes)
- Helm (helm)
- Oracle Cloud Infrastructure Cloud Controller Manager Module (oci-ccm)

---

#### [Use Quick Install to Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/42f9b19b-e254-42cf-885d-a80127d9d751)

Learn how to use Quick Install to install and configure Oracle Cloud Native Environment on Oracle Linux.

Oracle Cloud Native Environment Release 1.5.7 introduced the ability to use the Oracle Cloud Native Environment Platform CLI to perform a quick installation of itself. This is done using the `olcnectl` provision command on an installation host (the operator node).

This lab describes how to perform a quick installation using the simplest series of steps possible to get Oracle Cloud Native Environment and a Kubernetes cluster installed. This lab uses private CA Certificates. It is recommended for a production environment that you use your own CA Certificates.

---

#### [Provision Persistent Volumes Using File Storage Service on Oracle Cloud Native Environment](https://luna.oracle.com/lab/5d95fdca-c690-4ebf-8ac0-315ac095ac59)

Learn how to provision Persistent Volumes using File Storage service on Oracle Cloud Native Environment on Oracle Linux.

Oracle Cloud Native Environment ships with the ability to install the Oracle Cloud Infrastructure (OCI) Cloud Controller Manager (CCM). The CCM is OCI's implementation of the Kubernetes control plane component that links your Kubernetes cluster to OCI.  The OCI CCM project implements a Container Storage Interface (CSI) plugin for Kubernetes clusters that implements both OCI Block Volume Storage and OCI File Storage Service to store persistent data.

This lab will focus on OCI File System service to provide nfs-style cloud storage.

---

#### [Use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment](https://luna.oracle.com/lab/cdf43182-16c7-4c42-9a91-6052a5934184)

This tutorial shows how to create and use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment. Both Persistent Volumes and Persistent Volume Claims work together to provide persistence to any container-based applications deployed onto Oracle Cloud Native Environment. You will start by covering how to use Persistent Volumes initially, and then cover the use of Persistent Volume Claims.

---

#### [Upgrade to Oracle Cloud Native Environment 1.6](https://luna.oracle.com/lab/fa8fc61b-893c-4507-93a2-711540e9ace7)

Learn how to upgrade to Oracle Cloud Native Environment 1.6.

Administrators of an Oracle Cloud Native Environment deployment are aware that many of the components, such as Kubernetes, are regularly updated. The upgrade process updates these components to the most recent release allowing any new features to become available for users.

This tutorial will show how to upgrade an Oracle Cloud Native Environment Release 1.5 install to Release 1.6.

---

#### [Run KubeVirt on Oracle Cloud Native Environment](https://luna.oracle.com/lab/87d85c56-d929-45bc-aa8c-3f51cd584b2d)

Learn how to deploy and run KubeVirt on Oracle Cloud Native Environment.

KubeVirt is a virtualization technology to create and manage virtual machines in Kubernetes. Administrators create these virtual machines using the kubectl command and Kubernetes custom resource definitions (CRDs). As with any container image within Kubernetes, it requires persistent storage to maintain its state. Hence, our need for Rook and Ceph.

Rook is a cloud-native storage orchestrator platform that enables Ceph storage for our Kubernetes cluster. Rook deploys as a Kubernetes operator inside a Kubernetes cluster and automates the tasks to provision and de-provision Ceph-backed persistent storage using the Kubernetes Container Storage Interface (CSI).

While Ceph allows the creation of block and object storage, there also exists a shared file system storage. This type uses a CephFilesystem (CephFS) to mount a shared POSIX (Portable Operating System Interface) compliant folder into one or more pods. This storage type is similar to NFS (Network File System) shared storage or CIFS (Common Internet File System) shared folders.

This tutorial guides users on deploying KubeVirt with Ceph storage managed by Rook on Oracle Cloud Native Environment.

---

### Installation Tutorials

Each tutorial provides step-by-step procedures to complete specific tasks but does not provide an environment. Perform these tutorial steps on your own Oracle Linux environment.

#### [Use Operator Lifecycle Manager to Deploy a Kubernetes Operator on Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-olm/#introduction)

This tutorial shows you how install the Operator Lifecycle Manager module for Oracle Cloud Native Environment into a Kubernetes cluster, then deploy a Kubernetes operator.  The Operator Lifecycle Manager module installs Operator Lifecycle Manager into a Kubernetes cluster. Operator Lifecycle Manager manages the installation and lifecycle management of Kubernetes operators in a Kubernetes cluster.

---

{{< figure src="/img/ocne/OCNE-kubernetes-section.png" alt="Kubernetes section banner" >}}

## Kubernetes

### Kubernetes Videos

An open-source system for automating the deployment, scaling and management of containerized applications, Kubernetes provides the tools to build a cluster of systems to support the launching of containerized applications. These containers can be deployed across the cluster systems and scaled as needed.  

#### A Quick Tour of Kubernetes on Oracle Linux

- {{< youtube id="syBe1H-qe8U" title="A Quick Tour of Kubernetes on Oracle Linux YouTube video" >}}

#### Introducing Kubernetes Resources on Oracle Linux

- {{< youtube id="e5m3TlvM4y4" title="Introducing Kubernetes Resources on Oracle LinuxYouTube video" >}}

#### Install Minikube on Oracle Linux

- {{< youtube id="u1qY8ax0U44" title="Install Minikube on Oracle Linux YouTube video" >}}

### Kubernetes Labs

Each lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment.

#### [Run Kubernetes on Oracle Linux](https://luna.oracle.com/lab/01e69515-8cda-4d6e-89af-849f324c4b7f)

Learn to run Kubernetes on Oracle Linux.

This lab works with Kubernetes running within a compact Oracle Cloud Native Environment on Oracle Linux. The intent is not to be a 'one stop shop' for everything needed to administer a production deployment. Instead, it introduces the skills required to deploy a working sample application and covers the following:

- Examines the different Kubernetes components such as a Pod, Deployment, and Service
- Examines the different Kubernetes objects
- A walkthrough example of how to deploy and test a sample project

---

#### [Install Minikube on Oracle Linux](https://luna.oracle.com/lab/8b2f7860-3204-4cd3-8d55-3f6de9ca03c2)

Learn how to install and configure minikube with the podman driver on Oracle Linux.

Minikube is a popular tool for developers and administrators to run a fully functional Kubernetes cluster in their local environment.

Although Minikube is cross-platform, this tutorial only guides you through the installation and configuration of minikube with the podman driver.

---

#### [Introducing Kubectl on Oracle Cloud Native Environment](https://luna.oracle.com/lab/6c65a513-b161-47d2-b45c-92ca02e38dc0)

Learn the basics of using kubectl with Oracle Cloud Native Environment.

This lab introduces kubectl, a widely used command-line tool for interacting with a Kubernetes cluster. Beginning with why it is helpful to learn about it, the lab will also introduce some basic kubectl commands that help to understand any services deployed on a Kubernetes cluster, for example:

- location of the configuration file
- kubectl config
- kubectl get
- kubectl describe
- kubectl version

---

#### [Use Kubectl to Manage Kubernetes Clusters and Nodes](https://luna.oracle.com/lab/4b16d141-4825-4d54-98f3-ce7babbea45c)

Learn the basics of using Kubectl to manage Kubernetes Clusters and Nodes with Oracle Cloud Native Environment.

This lab builds on the basic commands introduced in a previous lab, Introducing Kubectl with Oracle Cloud Native Environment . If this is your first encounter using kubectl, you may find it beneficial to start there. This lab introduces how kubectl can manage individual Kubernetes Nodes and any application(s) deployed onto them. The specific areas of Node management introduced in lab are:

- Querying Cluster Information
- Querying Node information
- Deploying an example application (Nginx)
- Introducing new concepts such as:
  - Cordoning/Uncordoning and Draining Nodes
  - Taints and Tolerations

---
#### [Use ConfigMaps and Secrets with Oracle Cloud Native Environment](https://luna.oracle.com/lab/14984256-1691-4d7a-8468-6ff38b6253ad)

Learn how to create and use ConfigMaps and Secrets with Oracle Cloud Native Environment.

This Lab shows how to create and use ConfigMaps and Secrets with Oracle Cloud Native Environment. Both ConfigMaps and Secrets are used to define configuration data and have many similarities. You will start by covering how to use ConfigMaps, and then cover the use of Secrets.

---

{{< figure src="/img/quiz1.png" alt="ocne-kubernetes-quiz" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:BPJX2YO" target="_blank" >}}
Take the quiz
{{< /button >}}

---

{{< figure src="/img/ocne/OCNE-istio-section.png" alt="ISTIO section banner" >}}

## Istio

Operating as a service mesh for managing the interaction and operation of services in a microservices architecture. Istio coordinates communication between services, providing service discovery, load balancing, security, recovery, telemetry, and policy enforcement capabilities.

### Istio Lab

Each lab provides step-by-step procedures to complete specific tasks in an Oracle-provided free lab environment. Follow the procedures to connect to your Oracle Linux compute instance on Oracle Cloud Infrastructure and complete the labs. Alternatively, you can perform the lab steps on your own Oracle Linux environment.

#### [Enable Istio Proxy Sidecar Injection in Oracle Cloud Native Environment](https://luna.oracle.com/lab/6e667326-fd72-4e65-a5b5-8398c5eef960)

Learn how to enable Istio Proxy Sidecar Injection in Oracle Cloud Native Environment.

---

{{< figure src="/img/quiz1.png" alt="Oracle Cloud Native Environment Quiz section banner" >}}

Test your skills on what you have learned so far with this quiz.

> **Note:** To access the quiz you will need to create a Single Sign On account if you do not already have one.

{{< button href="https://apexapps.oracle.com/pls/apex/f?p=ST_QUIZ:200:0::::P200_QUIZ_KEY:DWXQQN7" target="_blank" >}}
Take the quiz
{{< /button >}}
