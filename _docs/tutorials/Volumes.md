---
title: Volumes
description: Provides information about volumes.
tags: [featured, quickstart]
# permalink: /volumes/
---
# Volumes
{: .no_toc }
---
In this page, you can find an explanation of how to create, edit, attach and detach volumes in Ventus Cloud Portal.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## About Volumes page
---

You can get to the volume page through the left-bar menu:

- In upper left corner click on menu icon

![](../../assets/img/Volumes/volume_page_1.png)

- And click on Volumes in opened menu

![](../../assets/img/Volumes/volume_page_2.png)

**Page content:**

Volume page consist of **headers** which include all needed information about volume, **Create button**, **side-bar menu** on the right side of page, **search bar** in front of create button:

![](../../assets/img/Volumes/volume_page_3.png)

Headers include:

- **Name:** The name of volume.
- **Region:** Shows in which region volume will be located.
- **Size:** Shows volume size.
- **Type:** Shows volume type.
- **Description:** Shows description to volume.
- **Status:** Shows in which status volume is. If volume is free, status will be `available` other way status will be `in-use`.

## Create volume
---

To create a volume, you need click on the create button in the right upper corner of volume page.

![](../../assets/img/Volumes/volume_page_4.png)

It will open **Create volume** window, which consist of required and optional fields for volume creation, and two buttons **Create Volume** and **Cancel**:

![](../../assets/img/Volumes/volume_page_5.png)

The required fields is: `Name`, `Size`, `Region`, `Type`.
Optional field is: `Description`.

First, you must specify volume name, size and region. Only after region was selected you can select volume type. And after you can fill description as needed.

- **Name** of volume can include all letter, numbers or symbols and must be not bigger than 255 characters. If volume was created by instance, name will be automatically filled with volume ID.
- **Size** can be specified  in the range from 10 GB to 1000 GB. Minimal available size `10 GB` is selected by default when you are opening create window.
- **Region** can be specified  from three available regions: `as`, `us`, `vs`. It depends on which region the created volume will be located.
- **Type** can be specified  from two available types: `RBD` and `__DEFAULT__`.
- **Description** can include all letter, numbers or symbols and must be not bigger than 255 characters.

When you specify all required fields click on **Create Volume** button.

![](../../assets/img/Volumes/volume_page_6.png)

Then, the "Create Volume" window will close and after a few seconds the volume you created will appear with the status `available`

**Cancel** button will close volume "Create Volume" window and will update all fields to their default state.

## Attach/Detach volume
---

<br>

- ### Attach volume

To attach volume you must select volume which has `available` status and click on side-bar menu.

![](../../assets/img/Volumes/volume_page_11.png)

In opened dropdown menu click on `Attach Volume` option.

{% include alert.html type="info" title="Note:" content="For volume which has status available Detach Volume button will be disabled." %}

![](../../assets/img/Volumes/volume_page_12.png)

It will open **Attach Volume** window, which contains a field for selecting the instance to which the volume will be attached, and two buttons **Attach Volume** and **Cancel**:

![](../../assets/img/Volumes/volume_page_13.png)

After you have selected an instance, click on **Attach Volume** button. 

![](../../assets/img/Volumes/volume_page_14.png)

Then, the "Attach Volume" window will close and after a few seconds the volume will be attached to instance and will go into status `in-use`

**Cancel** button will close "Attach Volume" window.

<br>

- ### Detach volume

To detach volume you must select volume which has `in-use` status and click on side-bar menu.

![](../../assets/img/Volumes/volume_page_15.png)

In opened dropdown menu click on `Detach Volume` option.

{% include alert.html type="info" title="Note:" content="For volume which has status in-use Attach Volume button will be disabled." %}

![](../../assets/img/Volumes/volume_page_16.png)

It will open confirmation window where user must confirm volume detach or cancel it.

![](../../assets/img/Volumes/volume_page_17.png)

**Cancel** button will close "Detach Volume" window.

**Confirm** button will close "Detach Volume" window and after a few seconds the volume will detach from instance and will go into status `available`.

{% include alert.html type="info" title="Note:" content="For volume which was created with instance Detach Volume button will be disabled." %}

## Edit volume
---
To edit volume you must click on it in side-bar menu of volume you want to edit.

![](../../assets/img/Volumes/volume_page_8.png)

In opened dropdown menu click on `Edit` option.

![](../../assets/img/Volumes/volume_page_18.png)

It will open **Edit volume** window, which consist of fields and options for volume you want to edit, and two buttons **Create Volume** and **Cancel**:

![](../../assets/img/Volumes/volume_page_20.png)

Options you can update:

- **Name** of volume can include all letter, numbers or symbols and must be not bigger than 255 characters.
- **Description** can include all letter, numbers or symbols and must be not bigger than 255 characters.
- **Bootable status** can be changed by clicking on **Bootable** checkbox in edit volume window. 

![](../../assets/img/Volumes/volume_page_19.png)

{% include alert.html type="info" title="Note:" content="Options that you can't change will be disabled in Edit Volume window." %}

After you have updated volume options, click on **Edit Volume** button. 

![](../../assets/img/Volumes/volume_page_21.png)

Then, the "Edit Volume" window will close and volume will be updated.

**Cancel** button will close "Edit Volume" window.


## Delete volume
---

There are two deferent ways to delete volume:

- Through the **side-bar menu** of volume
- Through the **checkbox** in front of volume Name.

- To delete volume through the side-bar menu you must click on it in right side of volume you want to delete.

![](../../assets/img/Volumes/volume_page_8.png)

In opened dropdown menu click on `Delete` option.

![](../../assets/img/Volumes/volume_page_9.png)

It will open confirmation window where user must confirm volume deletion or cancel it.

![](../../assets/img/Volumes/volume_page_10.png)

**Cancel** button will close "Delete Volume" window.

**Confirm** button will close "Delete Volume" window and after a few seconds the volume will be deleted.

 - To delete volume through checkbox you must click on it in front of volume Name of volume you want to delete.

![](../../assets/img/Volumes/volume_page_22.png)

When you select a volume, instead of the **Create** button, a **Delete** and **Cancel** buttons will appear in the upper right corner of the volume page.

![](../../assets/img/Volumes/volume_page_23.png)

**Cancel** button will cancel selection and return volume in default state.

**Delete** button will delete volume without confirmation.

Also, you can multi-delete volumes. For that select as more volumes as you need by clicking on their checkboxes. The counter in header will show you how many volumes you had selected.

![](../../assets/img/Volumes/volume_page_25.png)

Click **Delete** button as in previous action to delete selected volumes. Deletion will be done without confirmations.

![](../../assets/img/Volumes/volume_page_24.png)

## Details volume page
---

To get to the Volume details page you must click on volume name 

![](../../assets/img/Volumes/volume_page_26.png)

Then you will go to the **Volume details page** where contains more details information about volume like: `volume ID`, `bootable status`, `created/updated` time.

![](../../assets/img/Volumes/volume_page_27.png)

Also, there is a transition to the **Snapshots page** through link in header.

![](../../assets/img/Volumes/volume_page_28.png)