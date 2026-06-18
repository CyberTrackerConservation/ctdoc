---
layout: page
title: Data over USB
nav_order: 11
parent: CyberTracker Classic
permalink: /classic/data-over-usb/
---
# Downloading Data over USB

This page describes how to download data from an Android device to the CyberTracker desktop application using a USB cable. This is useful for offline-only scenarios.

## Before you start

Make sure CyberTracker is installed on both the Android device and the Windows desktop. See the [Download](/classic/download/) page if you need to install it.

## Step 1 — Connect the USB cable and set the connection type

When the device is connected, Android shows a USB connection notification. Tap it and choose **File transfer** (also called MTP on some devices).

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-2.png" /></td>
</tr>
</table>

{: .important }
If you do not change the connection type to **File transfer**, the desktop will not be able to see the device.

## Step 2 — Export the data on the device

1. Open CyberTracker on the device
2. Open the project you want to export data from
3. Tap the **Options** button
4. Go to the **Export data** tab
5. Tap the **Export** button

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-5.png" /></td>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-6.png" /></td>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-7.png" /></td>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-8.png" /></td>
</tr>
</table>

If you tap **SHOW EXPORTED DATA**, then you will see the data file. You can choose to share it as a CTX via another channel as needed.

## Step 3 — Download the data on the desktop
Open CyberTracker on the desktop and click **File → Download data over USB**. The data exported in the previous step will be downloaded and removed from the device.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-4.png" /></td>
</tr>
</table>

## Alternate method
The data is also exported to the `Download -> CyberTrackerData` folder as CTX files. You can manually copy this data using Windows Explorer and import it into CyberTracker via `File->Import data`.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/classic/data-usb-3.png" /></td>
</tr>
</table>
