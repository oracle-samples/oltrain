---
title: "Use Vertical Pod Autoscaling with Oracle Cloud Native Environment"
date: 2025-01-10
draft: false
summary: "Learn how to configure VerticalPodAutoscaler to scale the Pods resources on an Oracle Cloud Native Environment cluster."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/33a13919-65d4-4002-86a1-d5e3dbcc16aa)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-vpa)

## Details

The [**VerticalPodAutoscaler**](https://github.com/kubernetes/autoscaler/tree/master/vertical-pod-autoscaler)(VPA) is the Kubernetes component designed to optimize the allocation of CPU and memory resources available to deployed pods based on their usage. Unlike the *HorizontalPodAutoscaler*, the *VerticalPodAutoscaler* does not ship with Kubernetes by default. Instead, Kubernetes provides it as a separate project on [GitHub](https://github.com/kubernetes/autoscaler/tree/master/vertical-pod-autoscaler).

The Vertical Pod Autoscaler has three components:

- The VPA Recommender: This monitors current and past resource usage and provides recommendations for the CPU and memory request values the container should use. Its recommendations are periodically updated to provide continued adaptation as the workload requirements vary over time.
- The VPA Updater: Watches the deployment for pods using incorrect values based on their CPU and memory usage over time. It recreates pods by implementing the values suggested by the VPA Recommender only if `updateMode: Auto` is defined. The updated endeavors adapt to workload changes as smoothly as possible to minimize downtime.
- The VPA Admission Controller: Modifies the values used for CPU and memory based on the VPA recommendations suggested at pod creation. This approach ensures Kubernetes is not creating pods using resource limits set to high or low, even if these differ from the values defined in the deployment descriptor. Thus providing the most optimum resource values when deploying new pods.

### VPA Benefits

Kubernetes Vertical Pod Autoscaling provides the following:

- Reduces costs by allocating resources efficiently, thereby reducing excess costs related to unused CPU and memory resources for the cluster.
- Optimizes cluster resources by ensuring all pods deployed on the cluster have sufficient resources.
- Removes the need for administrators to benchmark deployments manually.

### VPA Limitations

Some limitations of the Kubernetes Vertical Pod Autoscaling include:

- Limited amount of data storage that has no persistence, which means any history is lost when a deployment restarts.
- Not compatible with Horizontal Pod Autoscaler. While similar to VPA, Kubernetes also provides a mechanism called **Horizontal Pod Autoscaling (HPA)**, which scales the number of pods deployed based on the CPU utilization metrics. Upstream documentation recommends that administrators not use HPA and VPA on the same resource metric.
- VPA is unaware of resources available to the cluster, so it may recommend more resources than are actually present. You can avoid this by tuning the VPA's *LimitRange* definition to the maximum present on your cluster.
- No awareness of other potential cluster bottlenecks. For example, network traffic and disk I/O, which may hinder its usefulness for data-intensive deployments.

Given these benefits and limitations, Kubernetes VPA is best used to provide automation for predictable variations in demand, but the overall cluster health still needs to be monitored.

### Objectives

In this tutorial, you will learn to:

- Install [Kubernetes Metric Server](https://github.com/kubernetes-sigs/metrics-server)
- Use Vertical Pod Autoscaling to enable deployments to respond to a changing workload

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and one worker node
