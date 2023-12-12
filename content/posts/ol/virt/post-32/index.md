---
title: "Install Keycloak"
date: 2023-10-18
draft: false
summary: "Learn to deploy Keycloak for providing authentication to applications and secure services using OAuth and SAML."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/752793ff-9f74-4bb0-b848-90c5bcae4388)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-keycloak)

## Details

Keycloak provides single sign-on functionality for web applications and RESTFUL web services.  A primary goal of Keycloak is to provide security features that developers can easily use to secure applications and services within their organizations, for example Single-Sign-On authentication.  Keycloak can also be integrated with existing LDAP and Active Directory servers.

Keycloak is based on standard protocols and provides support for User Federation, OpenID Connect, OAuth 2.0 and SAML and many more.  Keycloak provides both administrators, and users, with management consoles.  Users can update their passwords, profile details and setup two-factor authentication via the Account Managment Console.  Likewise administrators can use the Admin Console to manage all aspects of Keycloak's functionality, it's authorization policies, applications and manage users (including user's permissions and sessions).


### Objectives

These guides show how to deploy Keycloak on Podman, configure it with a datastore using a Podman volume to store the data outside of Podman.  Then demonstrate how to access Keycloak, create a new `Realm` then add a `User` to the newly created Keycloak `Realm`.  Finally the newly created `User` will log on to the Keycloak server's newly created `Realm` to demonstrate where a `User` could manage the Single Sign-On details.  The main steps are outlined below:

  - Install Podman
  - Configure a Podman network and volume
  - Deploy a Postgres database container
  - Deploy a Keycloak container using the Postgres container as a datastore
  - Create a new Keycloak `Realm` and `User`

> **Note:** A production deployment would most likely use either Podman secrets, or Kubernetes secrets, to obfuscate any passwords.  Neither of the scenarios are covered in this Lab.

### What Do You Need?

  - A client system with Oracle Linux installed
  - Access to the Internet
