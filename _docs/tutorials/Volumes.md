---
title: Volumes
description: Provides information about volumes.
tags: [featured, tutorial]
# permalink: /Volumes/
---

# Volumes

{: .no_toc }

In this page, you can find an explanation of how to create, edit, attach and detach volumes in Ventus Cloud Portal.

## Table of contents

{: .no_toc .text-delta }

1. TOC
   {:toc}

## About Volumes page

You can get to the volume page through the left-bar menu:

- In upper left corner click on menu icon

![](../../assets/img/Volumes/volume_page_1.png)

- And click on Volumes in opened menu

![](../../assets/img/Volumes/volume_page_2.png)

**Page content:**

Volume page consist of **headers** which include all needed information about volume, **Create button**, **side bar menu** on the right side of page, **search bar** in front of create button:

![](../../assets/img/Volumes/volume_page_3.png)

Headers include:

- **Name:** The name of volume.
- **Region:** Shows in which region volume will be located.
- **Size:** Shows volume size.
- **Type:** Shows volume type.
- **Description:** Shows description to volume.
- **Status:** Shows in which status volume is. If volume is free, status will be `available` other way status will be `in-use`.

## Create volume

To create a volume, you need clikc on the create button in the left upper corner of volume page.

![](../../assets/img/Volumes/volume_page_4.png)

The create button will open **Create volume** window, which consist of required and optional fields for colume creation:

![](../../assets/img/Volumes/volume_page_4.png)

The required fields is: `Name`, `Size`, `Region`, `Type`.
Optional field is: `Description`.

First of all you must specify volume name, size and region. Only after region was selected you can choose volume type. And after you can fill description as needed.

**Name** of volume can include all letter, numbers or symbols and must be not bigger then 255 characters. If volume was created by instance, name will be automaticly fill with volume ID.
**Size** can be specifed in the range from 10 GB to 1000 GB. Minimal availabel size `10 GB` is selected by default when you opening create window.
**Region** can be specifed from three available regions: `as`, `us`, `vs`. It depends on which region the created volume will be located.
**Type** can be specifed from two available types: `RBD` and `__DEFAULT__`.
**Description** can include all letter, numbers or symbols and must be not bigger then 255 characters.

**The Network Time Protocol (NTP)** is a networking protocol for clock synchronization between IT systems. NTP supports a monitoring service that allows administrators to query the server for traffic counts of connected clients via the 'monlist' command.

**Problem:**  
The NTP 'monlist' feature can be abused for DDoS reflection attacks against third parties.
