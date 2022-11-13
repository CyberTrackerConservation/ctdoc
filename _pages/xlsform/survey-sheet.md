---
layout: page
title: survey sheet
nav_order: 2000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/survey-sheet
has_toc: false
---
# **survey** sheet
The `bind::ct:parameters` JSON object in the **survey** sheet controls options for a single question or question group.

## contentPadding (integer)
Padding around the content area of the page.
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
      <td>{ "contentPadding": 4 }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>
