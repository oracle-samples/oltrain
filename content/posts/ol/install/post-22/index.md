---
title: "Create Custom Oracle Linux Images with Image Builder"
date: 2024-09-26
draft: false
summary: "Learn how to use the Image Builder tool from command line to create custom Oracle Linux images to deploy on cloud and bare metal systems."
tags: ["ol","lab","tutorial","ol-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/d2e7e00a-3477-47bc-bbaa-86e8adb40dd7)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-image-builder-custom-images)

## Details

In addition to downloading standard installation images for different platforms, you can generate your own custom Oracle Linux images with the Image Builder tool to install Oracle Linux.

All additional packages and customizations you plan to add to your new custom image are defined using a blueprint. The tool creates your custom composer image based on your blueprint and chosen image format, ready to deploy on various cloud and bare metal platforms. The custom images are stored in the tool and ready to be downloaded whenever needed.

The tool works from the command line or from the Image Builder page in the Cockpit web console.

This tutorial describes how to use the Image Builder tool from the command line to create ready-to-deploy custom Oracle Linux images.

### Objectives

In this tutorial, you will learn how to:

- Install the Image builder tool
- Create and configure blueprints
- Use blueprints to create composer images
- Download composer images from the tool
- View and download image log files and metadata
- Create custom image for cloud deployment
- Delete Images and Blueprints from the tool

### Prerequisites

- An Oracle Linux system
