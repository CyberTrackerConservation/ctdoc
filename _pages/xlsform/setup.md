---
layout: default
title: Initial setup
nav_order: 500
parent: Features
grand_parent: XlsForm
permalink: /xlsform/setup
has_toc: false
---
# Initial setup

### Add the `ct` namespace and the `bind::ct:parameters` column to the **settings** sheet
The `ct` namespace tells other XlsForm tools to ignore columns starting with `bind::ct:`.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>version</th>
      <th>namespaces</th>
      <th>bind::ct:parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>2022101001</td>
      <td>ct="http://cybertracker.org/xforms"</td>
      <td></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### Add the `bind::ct:parameters` column to the **survey** sheet
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
      <td>today</td>
      <td>today</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>Animal</td>
      <td></td>
    </tr>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>How many?</td>
      <td></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### Add the `bind::ct:parameters` column to the **choices** sheet
<table class="xlsTable">
  <thead>
    <tr>
      <th>list_name</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>animal</td>
      <td>lion</td>
      <td>Lion</td>
      <td></td>
    </tr>
    <tr>
      <td>animal</td>
      <td>elephant</td>
      <td>Elephant</td>
      <td></td>
    </tr>
    <tr>
      <td>animal</td>
      <td>rhino</td>
      <td>Rhino</td>
      <td></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>