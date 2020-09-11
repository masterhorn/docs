---
title: Security Guide
description: Provides information about security incidents and how to fix problems. the issues.
tags: [featured, tutorial]
# permalink: /Security_Guide/
---

# Security Guide

## {: .no_toc }

Our Security Guide provide further information on security incidents reported with e-mail Reports to Users and how to fix the issues.

The open services can be abused – or have already been actively abused – for DDoS reflection attacks against third parties.
Currently, incidents on the following openly accessible services are taken into account:

## Table of contents

{: .no_toc .text-delta }

1. TOC
   {:toc}

## NTP servers with 'monlist' enabled

---

**Defenition:**  
**The Network Time Protocol (NTP)** is a networking protocol for clock synchronization between IT systems. NTP supports a monitoring service that allows administrators to query the server for traffic counts of connected clients via the 'monlist' command.

**Problem:**  
The NTP 'monlist' feature can be abused for DDoS reflection attacks against third parties.
