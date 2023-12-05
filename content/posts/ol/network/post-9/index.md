---
title: "Create Network Bonds"
date: 2022-05-02
draft: false
summary: "Learn how to create a logical group interface by bonding multiple interfaces together using the nmcli and ip commands on Oracle Linux."
tags: ["ol","lab","tutorial","ol-network"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/fc37cd13-6a90-49df-adc1-6c3b40239265)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-nmcli-bond)

## Details

A network bond groups multiple physical network interfaces on a system into a single logical group interface and is connected to a network switch. Bonding can facilitate higher connection availability through redundancy by maintaining the connection if a link in the bond group fails. Also, the aggregation of the physical network interface provides higher throughput by load balancing the traffic across the interfaces in the bond.

### Objectives

This lab demonstrates using the Network Manager CLI (nmcli) utility to:

   - Create a bond interface
   - Add multiple physical interfaces as links in the bond interface group
   - Change the bond mode used for monitoring the status and the distribution of traffic across the bond interface links
   - Delete the bond interface

### Prerequisites

   - A cloud instance system with current release Oracle Linux installed


