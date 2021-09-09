---
layout: page
title: Offline maps
nav_order: 10
parent: SMART
permalink: /smart/offline-maps/
---
# Offline maps

By default, the “SMART Basemap” feature generates an offline map based on the map in SMART. If this is not sufficient, custom offline maps can be added to the SMART Mobile Package.
SMART Mobile supports MapBox (.mbtiles) and ArcGIS (.tpk, .vtpk) offline maps.
To enable them, on the Package dialog, select the “Basemap Settings” tab, then add layers from your machine.

![Image]({{ site.baseurl }}/assets/smart/offline-maps-1.png)

During the next package upload, these files will be available via the Layers menu (bottom left):

|:-------------|:-------------|
| ![Image]({{ site.baseurl }}/assets/smart/offline-maps-2.png) | ![Image]({{ site.baseurl }}/assets/smart/offline-maps-3.png) |

Note that it can be helpful to disable the online layers by selecting “None”. This will enable only the offline layers.

