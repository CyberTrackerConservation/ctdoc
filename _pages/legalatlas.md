---
layout: home
title: Legal Atlas
permalink: /legalatlas/
nav_order: 7450
---
# Legal Atlas
<img src="{{ site.baseurl }}/assets/legalAtlas/logo.svg" align="right" class="inline" style="width:15%;"/>
CyberTracker and SMART Mobile support [Legal Atlas](https://legal-atlas.net/) map packages. These packages contain polygons and metadata which is used to determine which laws apply in a particular location.

## Setup
CyberTracker and SMART Mobile can load a Legal Atlas map package (a zip file) directly. Copy it to your device and then use Settings->Offline Maps and add it. SMART Mobile also supports adding a Legal Atlas map package as an offline map layer.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/legalatlas/offline-maps-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/offline-maps-2.png" /></td>
</tr>
</table>

## Selecting a lookup location
Legal Atlas functionality is only available when Legal Atlas offline map layers are loaded. There are three ways to trigger a lookup:

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/legalatlas/map-pointer.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/map-current.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/smart-patrol.png" /></td>
</tr>
</table>

1. The magnifying glass appears on the map after a long press (pressing and holding down). This allows specifying a precise location for the lookup.

1. Using the `...` button in the lower right corner of the map page triggers a popup. The last option on the popup is "Legal Atlas" and this will use the current location for the lookup.

1. During a SMART patrol or survey, the control popup has a "Legal Atlas" button. This performs a lookup on the last known location. Typically this will be the current location.

## Navigating content

Once a lookup location has been chosen, a new page pops up with a navigation structure. Choosing list items navigates through the content.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-0.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-2.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-3.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/legalatlas/law-nav-5.png" /></td>
</tr>
</table>

**Note:**
1. Pressing the back on the top-most left back button returns you to the prior page.
1. Pressing the back button on the title bar navigates to the prior lookup page.