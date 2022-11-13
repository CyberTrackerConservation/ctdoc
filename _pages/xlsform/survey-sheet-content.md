---
layout: page
title: survey sheet - content
nav_order: 5000
parent: Features
grand_parent: XlsForm
permalink: /xlsform/survey-sheet-content
has_toc: false
---
# **survey** sheet - content
The content section is the middle part of the screen between the header and footer. By default it automatically selects a control for the question type, e.g. a date selector for a date question. By specifying a custom content object, more styles are available. This is especially useful for customizing lists.

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
      <td>select_one animal</td>
      <td>animal</td>
      <td>Select animal</td>
      <td>{ "content": { "style": "IconOnly", "itemHeight": 64, "columns": 3 } }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

## style (string)
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
- Value is ignored, but setting it activates a grid view.

Ignored otherwise.

## padding (integer)
Padding between grid items.

## columns (integer)
Number of columns for grids. Defaults to 2.

## lines (boolean)
Show lines between cells for grids. Defaults to true.

## border (boolean)
Show border around the outside of a grid. Defaults to false if contentPadding is 0, true otherwise.

## borderWidth (integer)
Border width for grid lines. Defaults to 2.

## fontSize (integer)
Size text font size. Defaults to 16.

## fontBold (boolean)
Set font to bold. Defaults to false.

## itemHeight (integer)
Set height of individual items. Defaults to 48.
