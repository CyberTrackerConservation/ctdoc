---
layout: page
title: settings sheet
nav_order: 1000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/settings-sheet
has_toc: false
---
# **settings** sheet
The `bind::ct:parameters` JSON object in the **settings** sheet contains options for the entire form.

## immersive (boolean, default `false`)
Setting this to `true` causes the form UI to use the wizard exclusively, i.e. this is more like CyberTracker Classic.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>{ "immersive": true }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

## colors (object)
The colors attribute specifies the color scheme used on the form. It follows the [Material Design](https://m2.material.io/design/color/the-color-system.html) system:
<br/><img src="{{ site.baseurl }}/assets/xlsform/material_design.png" />

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>{ colors: { "primary": "#6200EE", "accent": "#BB86FC" } }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>
