---
title: "Get Started with Git"
date: 2023-10-16
draft: false
summary: "Learn how to install and get started using Git on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6c55a20f-e751-4326-a157-b16770262346)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-git-start)

## Details

Git is a free and open-source Distributed Version Control System (DVCS) which is available for MacOS, MS Windows and Linux/Unix platforms. This lab only covers using Git on Oracle Linux, but the steps covered in this lab work for any platform.

How does Git work?  Git does not need a centrally located Git server to be fully functional. Instead, a simple project consists of a local folder on your computer containing files. Git then tracks any changes made to the directories and files contained within the project over time. It achieves this by storing the history and details of branches and commits locally  without requiring a network connection.

The ability to manage your code history and track these changes over time is why it is called a _version control system_. Notice the absence of '_distributed_'?  Being '_distributed_' requires a remotely hosted server to provide some of the more advanced features of a remotely hosted server such as GitHub.

Git is very powerful with a large feature set that assists development teams in tracking those changes. Git is most efficient when used at the command line - this may appear to be a barrier for some users. The command line can appear confusing at times, hopefully, this lab helps by providing an introduction showing how to install, configure and then start using Git on Oracle Linux.

> **Note:** This lab shows how to install and use Git locally. It does not cover using a remote repository, such as GitHub.

### Objectives

In this lab, you'll learn:

  - What Git is
  - How to install Git
  - How to create a Git repository
  - The basic commands to use with Git

### What Do You Need?

  - An Oracle Linux system.

