---
title: "Integrate LDAP User Management"
date: 2024-12-13
draft: false
summary: "Learn how to integrate LDAP user management with Oracle Linux Automation Manager."
tags: ["olam","lab","tutorial"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a03cfc90-4c3c-488d-9e66-ba514e00b619)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/olam-ldap)

## Details

Oracle Linux Automation Manager allows administrators to integrate LDAP for user management alongside the existing internal RBAC (role-based access control) source. Once configured, users logging in with an LDAP account automatically generate an Oracle Linux Automation Manager account and get assigned to a standard user or administrator organization.

### Objectives

In this tutorial, you'll learn how to:

- Create and configure accounts and groups in LDAP
  - *bind* account
  - *user* account
  - *superuser* group
  - *system_auditor* group
- Configure Oracle Linux Automation Manager to use LDAP
- Verify LDAP access
- Enable LDAPS

### Prerequisites

- A system with Oracle Linux Automation Manager installed.
- An available LDAP server, such as the open-source FreeIPA identity management server. 
