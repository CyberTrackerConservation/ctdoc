#---
layout: page
title: Snap location
nav_order: 1000
parent: Tutorials
grand_parent: XlsForm extensions
permalink: /xlsform/tutorial/1
has_toc: false
---
Snap location
=============
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Goal
This tutorial demonstrates configuring the **snapLocation** feature described in the [reference manual]({{ site.baseurl }}/xlsform/reference-manual/6#snaplocation).

## Requirements
- CyberTracker running on a Windows or Mac
- Excel or other XlsForm editor

## Steps
Follow the [Getting started]({{ site.baseurl }}/xlsform/tutorial/0) tutorial for set up.

### 1. Open the form
Open the `form.xlsx` file for the project.

### 2. Mark the `geopoint` question as `hidden` in the `appearance` column
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>appearance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geopoint</td>
      <td>my_location</td>
      <td>hidden</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### 3. Set the `bind::ct:save.snapLocation` column to `true`
CyberTracker also works with `TRUE`.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save.snapLocation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>text</td>
      <td>note</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table> 

### 4. Verify
In the example below, when the user presses **Save** then the location is taken automatically. 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-1a.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-1b.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-1c.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-1d.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-1e.png" /></td>
<td></td>
</tr>
</table>

## Form
[Download XlsForm]({{ site.baseurl }}/assets/xlsform/tutorial-1.xlsx)

## Demo
On desktop, copy this [link](https://cybertrackerwiki.org/applink?AhUEAP9wcm9qZWN0VWlkAP8ieGxzZm9ybV90dXRvcmlhbF8xIgAG_yJ3aWtpOi94bHNmb3JtL3R1dG9yaWFsLTEuanNvbiIA) to the clipboard and use the `File->Connect using clipboard link` option in CyberTracker.

On mobile, scan the QR Code below after installing CyberTracker. It will download and install the project.
<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/xlsform/tutorial-1-qrcode.png" /></td>
</tr>
</table>
