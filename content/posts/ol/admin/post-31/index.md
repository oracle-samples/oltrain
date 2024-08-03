---
title: "Get Started with Git"
date: 2023-10-16
draft: false
summary: "Learn how to install Git and start using it on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6c55a20f-e751-4326-a157-b16770262346)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-git-start)

## Details

Git is a free and open-source Distributed Version Control System (DVCS) available for MacOS, MS Windows, and Linux/Unix platforms. This tutorial covers using Git on Oracle Linux, but the steps covered in this tutorial work for any platform. 

How does Git work? Git does not need a centrally located Git server to be fully functional. Instead, a simple project consists of a local folder on your computer containing files. Git then tracks any changes made to the directories and files contained within the project over time. It achieves this by storing the history and details of branches and commits locally without requiring a network connection.

The ability to manage your code history and track these changes over time is why it is called a *version control system*. Notice the absence of *distributed*? Being *distributed* requires a remotely hosted server to provide some of the more advanced features of a remotely hosted server such as GitHub.

Git is very powerful, with an extensive feature set that assists development teams in tracking changes. It is most efficient when used at the command line, which may appear to be a barrier for some users. The command line can appear confusing at times. Hopefully, this tutorial will help by providing an introduction showing how to install and configure Git and then start using it on Oracle Linux. 

> **Note:** This tutorial shows how to install and use Git locally. It does not cover using a remote repository, such as GitHub.

### Objectives

In this tutorial, you'll learn how to:

  - Install Git
  - Create a Git repository
  - Use Git

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:

   - A non-root user account with sudo access
   - Access to the internet
