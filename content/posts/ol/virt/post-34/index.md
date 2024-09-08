---
title: "Deploy Quay in HA"
date: 2023-03-31
draft: false
summary: "Learn to set up and use a high-availability deployment of Project Quay Registry using Podman and HAProxy on Oracle Linux."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a63c2548-c459-457f-b3d1-123c99d90d89)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-quay-ha)

## Details

Project Quay is an open-source repository that stores and manages artifacts such as containers for use on cloud-native platforms. It offers these and many other features:

  - High availability registry
  - Vulnerability scanning, logging, auditing, notifications, and alerts
  - Role-based access control (RBAC)
  - Integration with OAuth support
  - Build automation integration with Git/GitHub/GitLab

As a container, it can be deployed on a Kubernetes cluster using an Operator or on Podman, providing a standalone or high-availability deployment. 

### Objectives

In this tutorial, you'll learn how to:

 - Access a 3-node Project Quay deployment
 - Verify basic Project Quay functionality works
 - Use the HAProxy Console to monitor Project Quay nodes

 > **Note:** The steps provided do not include configuring the registry using certificates. Therefore, configuring Project Quay in this specific way is recommended for non-production purposes or an internal/air-gapped environment only.

### Prerequisites

- Four Oracle Linux systems

- Each system should have Oracle Linux installed and configured with:
   - A non-root user account with sudo access
   - Access to the Internet
   - Firewall and ingress rules to allow TCP and/or HTTP traffic for the services

| Server Name | Role/Purpose                                                        | 
| ----------- | ------------------------------------------------------------------- | 
| *ol-node-01* | Hosts the HAProxy load balancer and the Postgres database           |
| *quay-01*, *quay-02*, *quay-03* | Hosts the Project Quay and Redis servers |
