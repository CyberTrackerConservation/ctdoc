---
layout: page
title: survey sheet - save
nav_order: 5000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/survey-sheet-save
has_toc: false
---
# **survey** sheet - save
The save object supports custom save behavior.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>How many?</td>
      <td>{ "save": { "geopoint": "location", "targets": [...], "track": [...] } }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

## geopoint (string)
Name of the question (survey sheet, name column) to store the current location. This triggers a location popup on save if the location question is not set. 

## targets (array of object)
An array of custom save targets. This creates a popup of possible target questions when the user presses **Save**:
<br/>
```json
{ "save": { "targets": [[{ "choice": "restart", "question": "animal"}, { "choice": "continue", "question": "count"}]] } }
```

On Save, the user will be presented with a popup with the options restart or continue. Depending on which is pressed, the new sighting will be started at that question.

'restart' and 'continue' are taken from the **choices** sheet in the 'saveTargets' list name.

### target array object 
The target is presented to the user as a target when save is pressed.

#### choice (string)
Choice name in a list called saveTarget in the choices sheet.

#### question (string)
Target question name. If the question is not relevant, then it will be ignored.

## track (array of object)
An array of custom track behaviors. Custom track timer configuration. These behaviors trigger depending on choices within the form. The track settings are updated on **Save**:
<br/>
```json
{ "save": { "track": [{ "condition": "${start_stop}='start'", "updateIntervalSeconds": 5, "distanceFilterMeters": 120 }, { "condition": "${start_stop}='stop'", "updateIntervalSeconds": 0 }]} }
```

### track array object
The track object allows configuration of the track timer.

#### condition (string)
An XlsForm expression which activates this option if matched, e.g. ${which_animal}='bee'

#### updateIntervalSeconds (integer)
Number of seconds between GPS readings. Set to 0 to disable the track timer.

#### distanceFilterMeters (integer)
Minimum distance between readings in meters. Optional - no distance filter is used if this is not specified.




