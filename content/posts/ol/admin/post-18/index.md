---
title: "Learn tmux"
date: 2021-07-20
draft: false
summary: "Learn to use tmux to control multiple terminal windows in a persistent session on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4dda7413-1a31-47bf-96c1-8fa6c306dc6b)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-tmux)

## Details

As a default, when your SSH connection terminates, any remote terminal sessions started by that connection also terminate. You can avoid that issue and reuse those sessions for yourself and others by using the tmux terminal multiplexer. You can also manage more complex tasks from a single SSH connection, as a terminal multiplexer can provide browser-style tabs for each task and even divide up your screen with multiple terminal sessions called panes.

In previous versions of Oracle Linux, you might have encountered a similar tool called `screen`. This tool has been around for years and is still available in the Oracle developer EPEL repository. However, we'll focus on and explore `tmux,` which Oracle ships in the base repository.

### Objectives

In this tutorial, you'll learn how to:

   - Connect and disconnect from a persistent tmux session
   - Display, hide, and switch between multiple terminals in the same tmux session
   - Manage several persistent tmux sessions

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet

