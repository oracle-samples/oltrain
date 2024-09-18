---
title: "Manage AppSteam Modules"
date: 2023-10-18
draft: true
summary: "Learn to manage and maintain user-space applications using AppStream modules on Oracle Linux."
tags: ["ol","lab","tutorial","ol-package"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/19feea85-3457-4e8d-bf4d-7f962ee0505f)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-dnf-modules)

## Details

DNF introduces the concepts of modules, streams, and profiles for managing different versions of software applications within a single OS release. Oracle Linux makes the content available separately from core OS packages and delivers it through two main repositories: BaseOS and Application Stream (AppStream). The BaseOS repository provides the core set of functionality in RPM packages, while the AppStream repository includes user-space applications, languages, databases, and other software packages.

Modules are a collection of RPM packages grouped together and installed together. A module can contain any of the following:

- packages with an application
- packages with the application's specific dependency libraries
- packages with documentation for the application
- packages with helper utilities<br><br>

Modules can have multiple streams, each containing a different version of packages and their dependencies. Think of module streams as virtual repositories within the physical repository. A module has only one of its streams enabled and active at any time, providing access to its packages. Each stream receives updates independently.

DNF frequently selects the stream with the latest version as the default stream and uses it when operations do not specify a particular stream or previously enable a different stream. Module streams can declare dependencies on the streams of other modules. This module dependency is irrespective of any package dependencies within the module. Streams can also contain packages from outside the module stream, which are usually from the BaseOS repository or the stream's dependencies.

Streams have multiple profiles that install a particular set of packages for a specific use case during the same DNF transaction. For example, DNF can use a profile to install a minimal or development configuration. A stream always has a default profile defined for installations when no other profile gets explicitly specified.

DNF can install packages using a module's profile with the `dnf module install` command or any of the module provided packages using the `dnf install PACKAGE-NAME` command.

When performing operations on modules, streams, and packages, keep in mind:

   - Enabling and installing a module stream might also require enabling and installing streams of other modules.
   - Disabling a stream of a module might also require turning off other module streams because a module stream does not remove packages automatically.
   - Removing a module stream removes all packages installed with a profile or stream, including their dependent packages.
   - Removing individual packages of the module stream doesn't turn off the stream. Leaving the module stream enabled allows for subsequent installations.
   - Switching an enabled stream of a module is the same as resetting the current stream and enabling a new stream.

### Objectives

In this lab, you'll learn to:

  - List all modules, streams, and profiles
  - Enable modules
  - Install modules
  - Install packages
  - Remove modules
  - Switch module streams
  - Disable modules

### What Do You Need?

  - An Oracle Linux system.

