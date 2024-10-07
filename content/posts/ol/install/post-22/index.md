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

For installing Oracle Linux, in addition to downloading standard installation images for different platforms, you can also generate your own custom Oracle Linux images with the Image Builder tool. 

All additional packages and customizations to be added to your new custom image are defined using a blueprint. The tool creates your custom composer image based on your blueprint and your chosen image format, ready to deploy on a variety of cloud and bare metal platforms. The custom images are stored in the tool, ready to be downloaded whenever you need.

The tool works from command line or from the Image Builder page in the Cockpit web console.

This lab describes how to use the Image Builder tool from command line to create ready to deploy custom Oracle Linux images.

### Objectives

In this lab you will practice how to:

- Install the Image builder tool
- Create and configure blueprints
- Use blueprints to create composer images
- Download composer images from the tool
- View and download image log files and metadata
- Create custom image for cloud deployment
- Delete Images and Blueprints from the tool

### Prerequisites

- Any Oracle Linux 8 system or later

