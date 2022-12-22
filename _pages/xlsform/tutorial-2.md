---
layout: page
title: Using Survey123
nav_order: 2000
parent: Tutorials
grand_parent: XlsForm extensions
permalink: /xlsform/tutorial/2
has_toc: false
---
Grid styles
===========
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Goal
This tutorial demonstrates how to activate location tracking with CyberTracker and Survey123. When done, an existing Survey123 form will be sending location data to an ArcGIS Online feature service.  

## Requirements
- Windows (64-bit) or Mac
- Excel or other XlsForm editor
- Account on ArcGIS Online
- Survey123 Connect 

## Steps
Follow the [Getting started]({{ site.baseurl }}/xlsform/tutorial/0) tutorial for set up.

### 1. Create a form using Survey123
- Login to an ArcGIS Online account
- Create and deploy a form with Survey123 - see the [online documentation](https://www.esri.com/survey123) to get started.

### 2. Install and launch 'ArcGIS Survey123 Connect' on the desktop
- [Link for the Windows version](https://apps.microsoft.com/store/detail/arcgis-survey123-connect/9PMST5C0DLST)
- [Link for the Mac version](https://apps.apple.com/us/app/arcgis-survey123/id993015031)

### 3. Use 'Open folder' to locate the XlsForm file
- Login and navigate to **My Survey Designs**
- Use the context menu and click on `Open folder`.
- Open the Excel file in the folder
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-1.png" /></td></tr>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-2.png" /></td></tr>
</table>

### 4. Create the hosted feature service on ArcGIS Online
- Open CyberTracker on the desktop and use the `Tools->Create ArcGIS location service` menu option

<table>
<tr><td><img width="240" src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-3.png" /></td></tr>
</table>

Fill in the login credentials and a service name. Click the **START** button to create the service.
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-4.png" /></td></tr>
</table>

When the service has been created, the dialog will display the service URL. Click **COPY TO CLIPBOARD**.
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-5.png" /></td></tr>
</table>

### 5. Update the 'settings' sheet
Return to Excel and update the `settings` sheet with the `namespaces`, `esriLocationServiceUrl` and `sendLocationInterval` columns.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>namespaces</th>
      <th>bind::ct:esriLocationServiceUrl</th>
      <th>bind::ct:sendLocationInterval</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>ct="http://cybertracker.org/xforms"</td>
      <td>https://services6.arcgis.com/.../FeatureServer</td>
      <td>30</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### 6. Create a track control question
Create a question in the form which controls the state of the track timer.  
