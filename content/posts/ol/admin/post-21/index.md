---
title: "Install NGINX"
date: 2021-06-05
draft: false
summary: "Learn how to install and configure NGINX on Oracle Linux."
tags: ["ol","lab","tutorial","ol-admin"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/54fa9d88-4243-4b4f-bae2-d52ec8cfb688)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-nginx)

## Details

NGINX is a lightweight HTTP/S server capable of higher performance and lower memory use than a typical Apache web server deployment. However, this performance gain comes at the cost of some functionality and flexibility. NGINX has also gained in popularity as a powerful proxy service capable of functioning as a direct HTTP proxy, a reverse proxy with caching, an SMTP, POP3, or IMAP proxy, or a generic TCP/UDP proxy. NGINX also provides load-balancing services with fault tolerance.

### Objectives

In this tutorial, you'll learn how to:

   - Install and enable the NGINX web server
   - Create a custom site
   - Enable SSL using a self-signed certificate

### Prerequisites

- Minimum of a single Oracle Linux system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Access to the Internet

> If using Oracle Cloud Infrastructure (OCI), create ingress security rules for destination ports 80, 443, and 8080 from anywhere.

