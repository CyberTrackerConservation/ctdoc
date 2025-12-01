---
layout: home
title: Goto applink
permalink: /goto-applink/
nav_order: 7600
---
# Goto Applink

CyberTracker supports a **goto target** that allows users to navigate to a location on the map. The location is typically set by tapping on a sighting or other map item and selecting the **Set goto** option. However, there is another way to configure the target using an applink.

### 1. Applink
Create an applink which will configure CyberTracker with the specified goto target. 

The applink format is: `https://cybertrackerwiki.org/applink?x=<base64-encoded-json>`

Where `<base64-encoded-json>` is:

```json
{
  "x": 1.234,
  "y": 5.678,
  "t": "Goto target title",
  "i": "https://wildlifeicons.org/icons/EarthRanger/activity/accident_rep.svg"
}
````

The above json therefore becomes: `https://cybertrackerwiki.org/applink?x=eyAieCI6IDEuMjM0LCAieSI6IDUuNjc4LCAidCI6ICJHb3RvIHRhcmdldCB0aXRsZSIsICJpIjogImh0dHBzOi8vd2lsZGxpZmVpY29ucy5vcmcvaWNvbnMvRWFydGhSYW5nZXIvYWN0aXZpdHkvYWNjaWRlbnRfcmVwLnN2ZyIgfQ`

Or, for SMART Mobile: `https://cybertrackerwiki.org/applink-smart?x=eyAieCI6IDEuMjM0LCAieSI6IDUuNjc4LCAidCI6ICJHb3RvIHRhcmdldCB0aXRsZSIsICJpIjogImh0dHBzOi8vd2lsZGxpZmVpY29ucy5vcmcvaWNvbnMvRWFydGhSYW5nZXIvYWN0aXZpdHkvYWNjaWRlbnRfcmVwLnN2ZyIgfQ`

Note:
1. The icon is optional
2. If the icon address does not start with `https`, then the system prepends `https://wildlifeicons.org/icons/`. This allows for shorter urls.

### 2. QR Code
Converting the above applink to a QR code and scanning it is also supported.
