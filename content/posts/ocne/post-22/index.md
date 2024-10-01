---
title: "Use ConfigMaps and Secrets"
date: 2024-10-01
draft: false
summary: "Learn how to create and use ConfigMaps and Secrets with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/14984256-1691-4d7a-8468-6ff38b6253ad)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-configmap)

## Details

A key advantage of containers is knowing your software executes on any computer without problems. Many applications use environment variables to control the application's runtime behavior, such as an API Key or environment variables. They may be hard-coded into a container, but doing so makes switching environments between a Production and Development environment difficult. Kubernetes addresses this by moving the application's configuration into an object called a ConfigMap comprised of a series of key-value pairs injected into the application's environment at runtime. The application then consumes these transparently as though they were environment values in their runtime environment.

### Objectives

In this tutorial, you'll learn how to:

- Use ConfigMaps and Secrets

### Prerequisites

- Installation of Oracle Cloud Native Environment
   - a single control and worker node
