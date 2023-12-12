---
title: "Learn tmux"
date: 2021-07-20
draft: false
summary: "Learn to use the tmux Terminal Multiplexer on Oracle Linux 8 or later."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4dda7413-1a31-47bf-96c1-8fa6c306dc6b)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/oracle-linux-tmux)

## Details

These guides provide step-by-step procedures for controlling multiple terminal windows in the same persistent session.

By default, terminating your SSH connection also terminates any remote terminal sessions started by that connection. If you use a terminal multiplexer, you can preserve those sessions for yourself and others to reuse. You can also manage more complex tasks from a single SSH connection, as a terminal multiplexer can provide browser-style tabs for each task, and even divide up your screen with multiple terminal sessions called "panes".

In previous versions of Oracle Linux, you might have encountered a similar tool called `screen`, but in this tutorial you will explore `tmux`. This tutorial is targeted at users of Oracle Linux 8 or later.

### Objectives

Upon completion of this Lab you will be able to:

- Connect and disconnect from a persistent tmux session
- Display, hide, and switch between multiple terminals in the same tmux session
- Manage several persistent tmux sessions

### What do you need?

- Any system with Oracle Linux 8

