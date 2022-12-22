---
layout: page
title: Using Survey123 tracks
nav_order: 2000
parent: Tutorials
grand_parent: XlsForm extensions
permalink: /xlsform/tutorial/2
has_toc: false
---
Using Survey123 tracks
===========
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Goal
This tutorial demonstrates how to activate location tracking with CyberTracker and Survey123. When completed, an existing Survey123 form will send location track data to an ArcGIS Online feature service. If you are not familiar with Survey123, start with the [portal](https://www.esri.com/survey123).

## Requirements
- Windows (64-bit) - Mac not yet supported
- Excel or other XlsForm editor
- Account on ArcGIS Online
- ArcGIS Survey123 Connect 

## Steps
It is recommended to follow the [getting started]({{ site.baseurl }}/xlsform/tutorial/0) tutorial to familiarize yourself with the tool. There are numerous online resources available.

### 1. Install and launch 'ArcGIS Survey123 Connect' on the desktop
[Link for the Windows Store version](https://apps.microsoft.com/store/detail/arcgis-survey123-connect/9PMST5C0DLST)

### 2. Create a new survey
Create a new survey or start with an existing survey.

You can use the **File** option and start with the [tutorial survey]({{ site.baseurl }}/assets/xlsform/tutorial-survey123-track.xlsx). This form still requires that the `bind::ct:esriLocationServiceUrl` column of the `settings` sheet be filled in before it will work (see step 4 below).
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-0.png" /></td></tr>
</table>

### 3. Use 'Open folder' to locate the XlsForm file
- Login and navigate to **My Survey Designs**
- Use the context menu and click on `Open folder`
- Open the Excel file in the folder
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-1.png" /></td></tr>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-2.png" /></td></tr>
</table>

### 4. Create the hosted feature service on ArcGIS Online
Launch CyberTracker on the desktop and use the `Tools->Create ArcGIS location service` menu option

<table>
<tr><td><img width="320" src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-3.png" /></td></tr>
</table>

Fill in the login credentials and a service name. Click the **START** button to create the service.
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-4.png" /></td></tr>
</table>

When the service has been created, the dialog will display the service URL. Click **COPY TO CLIPBOARD**.
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-5.png" /></td></tr>
</table>

Login to your ArcGIS Online account and verify that the service has been created:
<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-6.png" /></td></tr>
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
The track settings are updated when the user presses **Save** and are dependent on something the user entered in the form. 

Select a question which controls the state of the track timer. For example, add the following `select_one` question to the beginning of the form:

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one track_items</td>
      <td>track</td>
      <td>Configure track</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table class="xlsTable">
  <thead>
    <tr>
      <th>list_name</th>
      <th>name</th>
      <th>label</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>track_items</td>
      <td>start</td>
      <td>Start</td>
    </tr>
    <tr>
      <td>track_items</td>
      <td>stop</td>
      <td>Stop</td>
    </tr>
    <tr>
      <td>track_items</td>
      <td>nochange</td>
      <td>No change</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

Now create a JSON array which tells CyberTracker which setting to use. This is set in the `bind::ct:save.track` column of the `settings` sheet. 

In this example, the when `start` option is selected, then the track timer will be set to a 5 second interval. When the `stop` option is selected, the track timer will be stopped. 

`snapTrack` takes all outstanding point data (since the last snap) and creates a single polyline feature in the __Track Lines__ polyline layer. This is required otherwise the device will never remove point data that has been sent. 

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:save.track</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My form</td>
      <td>[{ "condition": "selected(${track}, 'start')", "updateIntervalSeconds": 5 }, { "condition": "selected(${track},'stop')", "updateIntervalSeconds": 0, "snapTrack": true }]</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>

### 7. Save, Update and Publish the form
- Save the form in Excel
- Click the `Update` button in Survey123 Connect
- Click the `Publish` button in Survey123 Connect

<table>
<tr><td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-7.png" /></td></tr>
</table>

### 8. Install the form in CyberTracker
Open CyberTracker and use the Connect page to connect to Survey123: 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8a.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8b.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8c.png" /></td>
</tr>
</table>

### 9. Create a start and stop sighting
- Use the **+** button to create a new sighting and after selecting `Start track`, tap the save button in the bottom right corner.
- Repeat and create a `Stop track` sighting.
- Click the **Submit** button in the bottom left corner of the survey **Home** page. Note that the **Yes** option on the submit dialog requires a long-press to confirm.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8d.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8e.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8f.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8h.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8i.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-8j.png" /></td>
</tr>
</table>

### 10. View the track data
View the location service data on ArcGIS Online.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-esri-9.png" /></td>
</tr>
</table>
