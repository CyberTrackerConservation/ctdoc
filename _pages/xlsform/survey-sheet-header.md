---
layout: page
title: survey sheet - header
nav_order: 3000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/survey-sheet-header
has_toc: false
---

# **survey** sheet - header
The header object supports custom header attributes. If no header object is specified, then the default header is used. By default, the header title is the question name.
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
      <td>{ "header": { "title": "Custom title", battery: true } }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

## textColor (string)
Color of title and subtitle text, e.g. "#3080FE".

## title (string)
Title text. Defaults to the question name.

## subtitle (string)
Subtitle text. Defaults to none and is therefore hidden.

## track (boolean)
Button in the top-right corner displays track timer state.

## battery (boolean)
Button in top-right corner displays battery state.
