---
title: "Use Role-Based Access Control"
date: 2025-08-06
draft: false
summary: "Learn how to use Role-Based Access Control (RBAC) with Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/88d99065-2b77-4ed1-8a64-a0c0260ab6a7)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-rbac)

## Details

As the number of deployments to your Kubernetes cluster increases, you may need help managing it. The [Kubernetes API](https://kubernetes.io/docs/concepts/overview/kubernetes-api/) provides the ability to add users and define their permissions to the cluster. 

Once the user has authenticated, Kubernetes verifies what actions the user is authorized to perform. [Role-Based Access Control (RBAC)](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) is natively supported by Kubernetes and enabled by default in Oracle Cloud Native Environment (Oracle CNE). Making it one of the access control methods commonly used. RBAC allows you to manage access to resources deployed to the Kubernetes environment by applying rules that restrict users' access to cluster resources. These rules can be either namespace-restricted using a *Role*, or cluster-wide using a *ClusterRole*.

You will find it helpful to have an understanding of the key components of Role-Based Access Control (RBAC) in Kubernetes, which are:

- **Roles:** A defined set of permissions that define allowed actions within a namespace.
- **RoleBindings:** Used to bind a Role to a user or service account within a namespace.
- **ClusterRole:** A defined set of permissions defining allowed actions across all namespaces in the cluster.
- **ClusterRoleBindings:** Used to bind a ClusterRole to a user or service accounts across all namespaces in the cluster.
- **Subjects:** These are users, groups, or service accounts that are bound to *Roles* or *ClusterRoles*.
- **Permissions:** These define the permitted actions a Role, or ClusterRole, can perform on a specified resource. They are associated with roles & cluster roles rather than users or service accounts.  

Another way to manage access to the Kubernetes cluster is [Attribute-Based Access Control (ABAC)](https://kubernetes.io/docs/reference/access-authn-authz/abac/), which allows finer tuning of policies compared to RBAC. But this is outside the scope of this tutorial.

This tutorial covers the basics of using RBAC to manage access to your Kubernetes cluster and demonstrates a simple use case.

For more information about Oracle Cloud Native Environment 2, please refer to the current [Release Documentation](https://docs.oracle.com/en/operating-systems/olcne/) site.

### Objectives

In this tutorial, you'll learn to:

- Create a Role to demonstrate restricting user permissions by namespace.
- Create a ClusterRole to demonstrate granting user permissions cluster-wide.

### Prerequisites

- Installation of Oracle Cloud Native Environment (Oracle CNE)
- A single control node and one worker node
