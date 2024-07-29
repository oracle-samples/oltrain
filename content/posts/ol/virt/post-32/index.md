---
title: "Install Keycloak"
date: 2023-10-18
draft: false
summary: "Learn how to deploy Keycloak to provide application authentication and secure services using OAuth and SAML."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/752793ff-9f74-4bb0-b848-90c5bcae4388)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-keycloak)

## Details

Keycloak provides authentication functionality for web applications and RESTFUL web services. Its primary goal is to provide security features that developers can easily use to secure applications and services within their organizations, such as Single-Sign-On. You can also integrate Keycloak with existing LDAP and Active Directory servers.  

Keycloak is based on standard protocols and supports user federation, OpenID Connect, OAuth 2.0, SAML, and many more. It provides both administrators and users with management consoles. Users can update their passwords and profile details and set up two-factor authentication via the Account Management Console. Likewise, administrators can use the Admin Console to manage all aspects of Keycloak's functionality, including authorization policies, applications, user permissions, and those users' sessions.

### Objectives

In this tutorial, you'll learn how to:

- Deploy Keycloak using Podman
- Configure Keycloak with a datastore using a Podman volume
- Access Keycloak:
   - Create a new realm
   - Add a user to the realm
   - Verify the user can log in

> **Note:** A production deployment would use either Podman or Kubernetes secrets to obfuscate passwords. This tutorial does not cover either scenario.

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Podman and cURL packages
    - Access to the Internet
