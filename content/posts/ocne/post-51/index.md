---
title: "Use Secrets"
date: 2025-05-21
draft: false
summary: "Learn how to use Secrets with Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5f5b5b18-263f-46a3-81e1-81d6b6386272)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-secrets)

## Details

Many applications have information, such as passwords, that only authorized users should access. This situation is where Kubernetes Secrets can help. They provide a way to securely manage sensitive data such as passwords, SSH, and API keys. Using secrets allows the separation of confidential data from the application's code, which reduces the risk of sensitive data being exposed or modified during the workflow of your Pods.

Before you start, it helps to know some basic details about Kubernetes Secrets:

- They must be present before being used by a Pod.
- Defined using a *KEY* and *VALUE* pair.
- Limited to a maximum size of 1MB to prevent them from using all of the kube-apiserver and kubelet memory.
- Define them as *immutable* to protect them from accidental or unwanted modification.

> **Important:** Kubernetes Secrets are not encrypted by default because they are only Base64-encoded and are stored unencrypted in etcd. So anyone with access to etcd can view or alter a Secret. Using Kubernetes Secrets can be made safe by using any of these methods:
>
> - Enable [Encryption at Rest](https://kubernetes.io/docs/tasks/administer-cluster/encrypt-data/) for Secrets.
> - Configure least-privilege access by using [RBAC authorization](https://kubernetes.io/docs/reference/access-authn-authz/rbac/).
> - Restrict access to secrets to specific containers.
> - Using an external secrets management service.

This tutorial covers the basics of Kubernetes Secrets and demonstrates a simple use case.

For more information about Oracle Cloud Native Environment 2, please refer to the current [Release Documentation](https://docs.oracle.com/en/operating-systems/olcne/) site.

### Objectives

In this tutorial, you'll learn to:

- Create a Secret
- View a Secret
- Decode a Secret
- Use a Secret to define an environment variable in a deployment

### Prerequisites

- Installation of Oracle Cloud Native Environment (Oracle CNE)
- A single control node and one worker node
