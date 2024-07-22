---
title: "Create Virtual Cloud Networks"
date: 2022-01-18
draft: false
summary: "Learn how to create a Virtual Cloud Network on Oracle Cloud Infrastructure."
tags: ["oloci","lab","tutorial","oloci-network"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5a3f5ad9-7931-43d8-bcdb-40884d6a100f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/create-vcn)

## Details

A Virtual Cloud Network, or VCN, is a software defined virtualized network in the Oracle Cloud Infrastructure that allows instances to communicate as if operating on a traditional network.

This lab takes you step by step through the manual process of building a new VCN without using the wizard.

The VCN includes components such as public and private subnets, route tables, internet gateways, DNS support, security lists, and more.

When creating a compute instance it must be associated with a subnet, so a VCN is created to provide network services to instances. It must be configured with at least one subnet so instances have a networking resource to use when being launched.

### Objectives

Upon completion of this Lab you will be able to:

- List the current VCNs associated with your compartment
- Launch the Virtual Cloud Network creation dialog in the web console
- Create a new VCN (without using wizard)
- Navigate and view the VCN details and its associated resources
- Create a subnet
- Add a CIDR block range of IP addresses
- Terminate a VCN

### Prerequisites

- Oracle Cloud Infrastructure web console

