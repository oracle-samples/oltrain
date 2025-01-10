---
title: "Use Horizontal Pod Autoscaling"
date: 2024-12-10
draft: false
summary: "Learn how to configure HorizontalPodAutoscaler to scale the number of Pods on an Oracle Cloud Native Environment cluster."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/c3ff7b1c-22f1-485f-af1e-f0677380ef1e)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-hpa)

## Details

The [**HorizontalPodAutoscaler**](https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/)(HPA) is the Kubernetes object for managing horizontal pod autoscaling. We refer to it as horizontal scaling because it allows Kubernetes to automatically deploy more Pods to match any variations to the incoming workload, such as the number of users making requests. Once the demand abates, HPA can scale the number of deployed Pods back down again. Kubernetes administrators can apply HPA to workload resources such as a *Deployment* or a *StatefulSet* as they include support for the [`scale` subresource](https://kubernetes.io/docs/tasks/extend-kubernetes/custom-resources/custom-resource-definitions/#scale-subresource). Not all Kubernetes objects support the `scale` subresource, one of which is a *DaemonSet*. A `scale` subresource allows the number of replicas to be altered depending on their current state.

### Benefits of HPA

Kubernetes Horizontal Pod Autoscaling helps by providing the following:

- Automatically increase the number of Pods deployed to meet sustained changes to incoming workload.
- Contributes to cost savings by automatically reducing the number of Pods as external demand reduces.
- Monitors the Kubernetes cluster's metrics to ensure deployed applications remain available.
- Allows you to configure expected capacity needs for both normal and busy workloads.

### Limitations of HPA

Some limitations of the Kubernetes Horizontal Pod Autoscaling include:

- It does not work with a *DaemonSet*.
- It only works if your cluster has sufficient resources, allowing it to add more Pods.
- HPA cannot scale the Kubernetes cluster nodes if the current cluster runs out of capacity.
- The CPU and Memory limits need to be tuned to prevent Pods from unexpectedly terminating if you set them too low or, conversely, wasting resources that could be used for other deployments if they are set too high.
- It does not consider other potential bottlenecks, such as network I/O, disk I/O, or disk space.

Given these benefits and limitations, Kubernetes HPA is best used to provide automation for predictable variations in demand, but the overall cluster health still needs to be monitored.

While similar to HPA, Kubernetes also provides a mechanism called **Vertical Pod Autoscaling (VPA)**, but administrators would use it to adjust the available CPU and Memory resources to existing Pods in a deployment rather than changing the number of Pods deployed. Upstream documentation recommends that administrators not use HPA and VPA on the same resource metric.

### Objectives

In this tutorial, you will learn to:

- Install [Kubernetes Metric Server](https://github.com/kubernetes-sigs/metrics-server)
- Use Horizontal Pod Autoscaling to enable deployments to respond to a changing workload

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and one worker node
