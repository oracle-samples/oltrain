---
title: "Set up Gluster Storage"
date: 2021-08-21
draft: true
summary: "Learn how to set up Gluster Storage"
tags: ["ol", "lab", "tutorial", "ol-storage"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4de49ca0-6b00-4c69-95a7-a60a4b21ab78)

:spiral_notepad: [Tutorial](https://docs.oracle.com//en/learn/gluster-oracle-linux)

## Details

The following tutorial describes how to install and set up Gluster Storage for Oracle Linux across multiple nodes that are running Oracle Linux 8 or later.

### Objectives

In this tutorial, you will learn how to:

- Enable access to Gluster repos and packages and install Gluster server packages
- Prepare each node to work as a Gluster storage node
- Create a storage pool
- Create volumes
- Test and mount a Gluster volume

### Prerequisites

The tutorial uses the following system:

- At least 4 Oracle 8 systems, 3 to constitute the nodes of a Gluster pool and 1 to function as a Gluster client.
- Block storage assigned to the systems to be used with Gluster. Look here for information about [adding block storage to Oracle Cloud Infrastructure instances](https://docs.oracle.com/en-us/iaas/Content/Block/Tasks/attachingavolume.htm)
