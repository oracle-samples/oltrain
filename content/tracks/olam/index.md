---
title: "Oracle Linux Automation Manager"
date: 2020-08-17
draft: false
description: "Welcome to Oracle Linux Automation Manager Track"
summary: "This track provides free training to help introduce you to Oracle Linux Automation Manager and improve your skills with its automation tools.  The Oracle Linux Automation Engine is an automation tool for deploying software, configuring systems, and orchestrating tasks such as upgrades and updates, in the form of playbooks.  Oracle Linux Automation Manager provides features that allow your organization to effectively manage infrastructure configuration through a browser user interface."
tags: ["olam","ansible"]
slug: "olam"
showRecent: false
showDate: false
showLikes: false
showViews: false
showEdit: false
showReadingTime: false
showAuthor: false
showDateUpdated : false
sharingLinks : false
hideFeatureImage: false
showHero: false
istrack: true
cascade:
  showDate: false
  showAuthor: false
  invertPagination: true
aliases:
- /OLAM/olam.html
- /olam/olam/
---

{{< figure src="/img/olam/OLAM-banner.jpg" alt="Oracle Linux Automation Manager Track" >}}

---

{{< lead >}} Oracle Linux Automation Manager is a task engine and Web interface for scheduling and running Oracle Linux Automation Engine playbook tasks on the inventories the playbooks interact with. The Oracle Linux Automation Engine is an automation tool for deploying software, configuring systems, and orchestrating tasks such as upgrades and updates, in the form of playbooks. {{< /lead >}}

---

{{< figure src="/img/olam/OLAM-banner-v2.png" alt="Oracle Linux Automation Manager section banner" >}}

## Oracle Linux Automation Manager

### Labs

Practice your skills with Oracle Linux Automation Manager with these free hands on labs.

#### [Install Oracle Linux Automation Manager on Oracle Linux](https://luna.oracle.com/lab/ecf924b0-a2e1-49eb-8700-8c8bea5d7502)

Learn how to install the Oracle Linux Automation Manager on Oracle Linux.

---

#### [Get Started with Oracle Linux Automation Manager](https://luna.oracle.com/lab/4a1dcd6e-231c-4724-ae52-8d56431a2888)

Learn how to setup and use Oracle Linux Automation Manager.  Oracle Linux Automation Manager provides features allowing your organization to effectively manage infrastructure configuration through a browser-based user interface.  By the end of this tutorial, you'll have a working Oracle Linux Automation Manager installation ready to run more complex playbooks.

---

#### [Upgrade to Oracle Linux Automation Manager](https://luna.oracle.com/lab/6c7124cc-474f-4dd4-89fa-9beb536c71f5)

Learn how to upgrade an Oracle Linux Automation Manager Release 1 installation to Release 2.  Existing administrators of Oracle Linux Automation Manager are familiar with its all-in-one single-instance deployment.  Oracle Linux Automation Manager allows administrators to upgrade their existing deployments and later migrate the upgraded instance into a clustered deployment. When upgrading, the instance converts to a single-host deployment and configures itself as a hybrid node.

---

#### [Migrate Oracle Linux Automation Manager to a Clustered Deployment](https://luna.oracle.com/lab/d1847f91-0cdc-41b8-afc4-eb6d0ccd40c2)

Learn how to migrate a single-host Oracle Linux Automation Manager installation to a clustered deployment with a remote database.  Whether upgrading from a previous release or starting with a single host installation, both environments can migrate to a clustered deployment. Administrators need to plan their topology before migrating, as the cluster may consist of a combination of Control Plane and Execution Plane nodes and a remote database.

---

#### [Integrate LDAP User Management with Oracle Linux Automation Manager](https://luna.oracle.com/lab/a03cfc90-4c3c-488d-9e66-ba514e00b619)

Learn how to integrate LDAP user management with Oracle Linux Automation Manager.

Oracle Linux Automation Manager allows administrators to integrate LDAP for user management alongside the existing internal RBAC (role-based access control) source. Once configured, users logging in with an LDAP account automatically generate an Oracle Linux Automation Manager account that assigns to an organization as a standard user or administrator.  By the end of this tutorial, you'll have a configured Oracle Linux Automation Manager that allows users to log in using their LDAP credentials.

---

#### [Use OCI Ansible Collection with Oracle Linux Automation Manager](https://luna.oracle.com/lab/b69c86cf-962a-40a9-8f3c-7a9018f4dc4b)

Learn how to use the OCI Ansible Collection with Oracle Linux Automation Manager.

The Oracle Cloud Infrastructure (OCI) Ansible Collection provides an easy way to provision and manage resources in the Oracle Cloud using Ansible.  This tutorial shows how to use this collection in Oracle Linux Automation Manager and interacts with an Oracle Cloud tenancy.

---

#### [Use Hop Nodes on Oracle Linux Automation Manager](https://luna.oracle.com/lab/c4780f15-bd17-468d-9133-3eba9bc0ff2a)

Learn how to use a hop node in Oracle Linux Automation Manager.  Oracle Linux Automation Manage supports a service mesh technology based on the upstream [receptor](https://receptor.readthedocs.io/en/latest/#xd_co_f=NjUzNDIzODAtMTcwNy00YzFlLTgxMDItNTM2YjIwZjBkMmQ0~) project.

The service mesh links controller, hop, and execution nodes into an overlay network through a daemon-based receptor application.  Oracle Linux Automation Manager introduces the hop node as part of the service mesh. This node type allows relaying tasks from control plane nodes to execution nodes on remote or restricted networks in the same way SSH uses a jump host. This implementation enables running jobs across different execution nodes and moving tasks closer to the systems needing automation.  To help automate the cluster installation on your hardware, check out the playbook in the [Oracle Linux Automation Manager](https://github.com/oracle-samples/ansible-collections/tree/main/playbooks/OLAM/cluster-plus-hop-node) section of the [ansible-collections project](https://github.com/oracle-samples/ansible-collections).

---

#### [Manage KVM Virtual Machines using Oracle Linux Automation Manager](https://luna.oracle.com/lab/3e869b97-6f71-46fa-a979-e0c8bf81d7d2)

Learn how to use the libvirt community collection to manage KVM virtual machines with Oracle Linux Automation Manager.

The community.libvirt collection provides libvirt modules and plugins supported by the Ansible libvirt community. These modules and plugins help manage virtual machines (VMs) and containers using the libvirt API.  This tutorial shows how to use this collection in Oracle Linux Automation Manager and interacts with an Oracle Linux instance running KVM.

---

#### [Setup HAProxy to Load Balance an Oracle Linux Automation Manager Cluster](https://luna.oracle.com/lab/1d19c310-b6d6-40a9-aa2b-44dee29a8f31)

Learn how to configure HAProxy to Load Balance an Oracle Linux Automation Manager Cluster.

Oracle Linux Automation Manager supports a cluster deployment of multiple control and execution nodes. With the control nodes acting as the entry point into the cluster, how does an administrator manage the traffic across these nodes? That is where a load balancer becomes beneficial. A load balancer efficiently distributes incoming network traffic across a group of backend servers or the control nodes in this solution. A load balancer ensures the Oracle Linux Automation Manager infrastructure is highly available and reliable and performance does not degrade.

---

#### [Build Custom Execution Environments with Oracle Linux Automation Manager Builder Utility](https://luna.oracle.com/lab/b54dddd3-661b-43af-afae-192e5fbdab07)

Learn to build custom execution environments for Oracle Linux Automation Manager.

The Builder utility is a tool based on the upstream ansible-builder project for generating custom execution environments for Oracle Linux Automation Manager.

---

#### [Manage Execution Environments in Oracle Linux Automation Manager Private Automation Hub](https://luna.oracle.com/lab/3e9f93ad-a33a-446a-aef5-4d6eb54e70af)

Learn to manage execution environments with Private Automation Hub.

The Private Automation Hub is an Oracle Linux Automation Manager feature based on the upstream Galaxy-NG project for managing collections, execution environment images, and other curated content locally within a customer's infrastructure.

---

#### [Use Custom Execution Environment with Oracle Linux Automation Manager](https://luna.oracle.com/lab/9b8e3edf-72c0-4e01-9b66-b27eb1002a47)

Learn to deploy and configure a custom execution environment in Oracle Linux Automation Manager for running jobs.

Through the use of a custom execution environment (ee), Oracle Linux Automation Manager can leverage playbooks containing collections and other resources not available with the default `olam-ee` image.

---

{{< figure src="/img/olam/OLAM-engine-section.png" alt="Oracle Linux Automation Engine section banner" >}}

## Oracle Linux Automation Engine

### Labs

Practice your skills with Oracle Linux Automation Manager Engine with these free hands on labs.

#### [Write a Playbook with Oracle Linux Automation Engine](https://luna.oracle.com/lab/27118507-76a6-4116-8ae3-eecc5314531e)

Learn to write a playbook using the Oracle Linux Automation Engine.

The Oracle Linux Automation Engine, a component of Oracle Linux Automation Manager, is an automation tool for deploying software, configuring systems, and orchestrating tasks, such as upgrades and updates, in the form of playbooks. Initially using the ansible package, Oracle Linux Automation Engine now stems from the open-source ansible-core software package.

---

#### [Automate Setup of Oracle Linux with Oracle Linux Automation Engine](https://luna.oracle.com/lab/56b90194-88ab-421e-bc93-2ac708dce6ba/)

Learn how to use Oracle Linux Automation Engine to perform the initial configuration of an Oracle Linux instance.  This lab provides a playbook for automating the initial setup of Oracle Linux using the configuration management tool Oracle Linux Automation Engine.

---

#### [Configure Podman Containers with Oracle Linux Automation Engine](https://luna.oracle.com/lab/6154cf89-6a6e-45b3-98ad-635979b953e8)

Learn how to use Oracle Linux Automation Engine to deploy Podman Containers on Oracle Linux.  This lab guides you through creating a playbook for installing Podman and running an Oracle Linux container using the configuration management tool Oracle Linux Automation Engine.

---

#### [Use an OCI Dynamic Inventory with Oracle Linux Automation Engine](https://luna.oracle.com/lab/95a9fc4b-56a4-4b89-b8f1-b90489df5340)

Learn to use the OCI Dynamic Inventory with Oracle Linux Automation Engine. Oracle Linux Automation Engine, the open-source software for provisioning and configuration management, uses an inventory file to work against managed nodes or hosts in your infrastructure. This inventory file contains a list of servers, their IP addresses, and other optional connection information.

A static inventory file works well if your infrastructure hardly changes.  However, your infrastructure is likely in constant flux when using the cloud. Therefore it would be great to have a way to have your inventory dynamically updated as hosts come and go.
