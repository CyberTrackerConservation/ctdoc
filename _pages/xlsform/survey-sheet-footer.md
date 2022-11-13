---
layout: page
title: survey sheet - footer
nav_order: 4000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/survey-sheet-footer
has_toc: false
---
# **survey** sheet - footer
The footer object supports custom control buttons, e.g. back, next, save, etc. If no footer object is specified, then the default control is used.

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
      <td>{ "footer": { "options": true, "map": false, "save": true" } }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

## options (boolean)
Show **options** button in immersive mode. Show **index** button in non-immersive mode. Default is true.

## map (boolean)
Show **map** button. Default is true.

## save (boolean)
Show save button. Default is false.

## next (boolean)
Show next button. Default is true, if there is a next page.
