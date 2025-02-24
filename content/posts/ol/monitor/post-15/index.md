---
title: "Performance Co-Pilot"
date: 2024-05-15
draft: false
summary: "Learn how to use Performance Co-Pilot on Oracle Linux."
tags: ["ol","lab","tutorial","ol-monitor"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/77c25cd0-139e-4a52-a6f6-0f14c628d40f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-pcp)

## Details

Performance Co-Pilot (PCP) collects OS and network metrics that you can use to diagnose performance issues. PCP is a distributed architecture with collector hosts and monitor hosts.

- PCP refers to the monitored hosts as collector hosts. These hosts require a Performance Metrics Domain Agent (PMDA), which is responsible for collecting performance measurements. The Performance Metrics Collector Daemon or `pmcd` controls all PMDAs on the same hosts.

- PCP monitor hosts display data collected from hosts, or archives, that have the PCP collector installed. The core PCP package includes many monitor tools.

### Objectives

In this tutorial, you will learn:

- Configure one Oracle Linux host as a PCP collector and monitor
- Use PCP monitoring tools on a single host
- Configure remote monitoring of a second Oracle Linux host
- Monitor performance with pmchart GUI

### Prerequisites

- Two (2) Oracle Linux 9 systems
