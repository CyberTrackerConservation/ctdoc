---
layout: default
title: Reference
nav_order: 200
parent: XlsForm
permalink: /xlsform/reference
has_toc: false
---
# Reference
{: .no_toc }

[XlsForm](https://xlsform.org) supports an [extension system](https://xlsform.org/#advanced-use-and-extensibility). CyberTracker leverages this system to provide customizations. These extensions are invisible to XlsForm tools, so they only affect the behavior of CyberTracker.

[Download a simple example]({{ site.baseurl }}/assets/xlsform/simple_form.xlsx)

Table of Contents
{: .no_toc .text-delta }

{:toc}
- TOC

## Initial setup
### Create the namespace
The `ct` namespace tells other XlsForm tools to ignore columns starting with `bind::ct:`.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>version</th>
      <th>namespaces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>2022101001</td>
      <td>ct="http://cybertracker.org/xforms"</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

## Form configuration - `settings` sheet

### immersive
Setting this to `true` causes the form UI to use the wizard exclusively, i.e. this is more like CyberTracker Classic. Default is `false`. `TRUE` and `FALSE` values also work.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:immersive</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### colors (object)
The colors attribute specifies the color scheme used on the form. It follows the [Material Design](https://m2.material.io/design/color/the-color-system.html) system:
<br/><img src="{{ site.baseurl }}/assets/xlsform/material_design.png" />

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:colors</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>{ "primary": "#6200EE", "accent": "#BB86FC" }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

## Header - `survey` sheet
The header object supports custom header attributes. If no header object is specified, then the default header is used. By default, the header title is taken from the question label.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:header</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>How many?</td>
      <td>{ "title": "Custom title", battery: true }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### textColor (string)
Color of title and subtitle text, e.g. "#3080FE", "red", "green", etc.

### title (string)
Title text. Defaults to the question label.

### subtitle (string)
Subtitle text - hidden if empty. Defaults to empty.

### track (boolean)
Button in the top-right corner displays track timer state.

### battery (boolean)
Button in top-right corner displays battery state.

## contentPadding (integer)
Padding around the content area of the page.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:contentPadding</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>How many?</td>
      <td>16</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

## Content - `survey` sheet
The content section is the middle part of the screen between the header and footer. By default it automatically selects a control for the question type, e.g. a date selector for a date question. By specifying a custom content object, more styles are available. This is especially useful for customizing lists.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:content</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>Select animal</td>
      <td>{ "style": "IconOnly", "itemHeight": 64, "columns": 3 }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### style (string)
For **select_one** questions:
- IconOnly
- TextOnly
- TextBesideIcon
- TextUnderIcon

For **select_multiple** questions:
- IconInlay
- IconOnly
- TextOnly
- TextBesideIcon

For **range** questions:
- Grid

Ignored for other question types.

### padding (integer)
Padding between grid items.

### columns (integer)
Number of columns for grids. Defaults to 2.

### lines (boolean)
Show lines between cells for grids. Defaults to true.

### border (boolean)
Show border around the outside of a grid. Defaults to false if contentPadding is 0, true otherwise.

### borderWidth (integer)
Border width for grid lines. Defaults to 2.

### fontSize (integer)
Size text font size. Defaults to 16.

### fontBold (boolean)
Set font to bold. Defaults to false.

### itemHeight (integer)
Set height of individual items. Defaults to 48.

## Footer - `survey` sheet
The footer object supports custom control buttons, e.g. back, next, save, etc. If no footer object is specified, then the default control is used.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>{ "options": true, "map": false, "save": true" }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### options (boolean)
Show **options** button in immersive mode. Show **index** button in non-immersive mode. Default is true.

### map (boolean)
Show **map** button. Default is true.

### save (boolean)
Show save button. Default is false.

### next (boolean)
Show next button. Default is true, if there is a next page.

## Save settings - `survey` sheet
The save object supports custom save behavior.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>{ "geopoint": "location", "targets": [...], "track": [...] }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### geopoint (string - name of geopoint question)
Creating a `geopoint` question type will prompt the user to enter a location. However, it is useful to snap the location only at save time. Setting this attribute to the name of the geopoint question will trigger a location popup (if the location is not already set).

To make the question invisible, either set the `label` for the geopoint question to empty, or set the `bind::ct:hidden` column to `true`. Using the hidden property allows the form to be compatible with other data capture tools. 

### targets (array of save targets)
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>{ "targets": [[{ "choice": "restart", "question": "animal"}, { "choice": "continue", "question": "count"}]] }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>
On save, the user will be presented with a popup with the options **restart** or **continue**. Depending on which is selected, a new sighting will be created starting at that question.

Note that **restart** and **continue** are taken from the `choices` sheet in the **saveTargets** list name.

#### choice (string)
Choice name in a list named `saveTarget` in the `choices` sheet. Choices are used because they can be localized.

#### question (string)
Target question name. If the question is not relevant, then this choice will be ignored.

### track (array of track configurations)
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>{ "track": [{ "condition": "${start_stop}='start'", "updateIntervalSeconds": 5, "distanceFilterMeters": 120 }, { "condition": "${start_stop}='stop'", "updateIntervalSeconds": 0 }] }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>
On Save, it is possible to change the location track configuration. The behavior which triggers is dependent on choices within the form. 

#### condition (string)
An XlsForm expression which activates this option if matched, e.g. ${which_animal}='bee'

#### updateIntervalSeconds (integer)
Number of seconds between GPS readings. Set to 0 to disable the track timer.

#### distanceFilterMeters (integer)
Minimum distance between readings in meters. Optional - no distance filter is used if this is not specified.
