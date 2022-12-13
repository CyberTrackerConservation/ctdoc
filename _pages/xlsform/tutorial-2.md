#---
layout: page
title: Grid styles
nav_order: 2000
parent: Tutorials
grand_parent: XlsForm extensions
permalink: /xlsform/tutorial/2
has_toc: false
---
Grid styles
===========
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Goal
This tutorial demonstrates various built-in grid styles for select_one, select_multiple and range lists.

## Requirements
- CyberTracker running on a Windows or Mac
- Excel or other XlsForm editor 

## Steps
Follow the [Getting started]({{ site.baseurl }}/xlsform/tutorial/0) tutorial for set up.

### 1. Open the form
Open the `form.xlsx` file for the project.

### 2. Add images to choices
Unzip the icons (see above) into the project folder (under CTProjects/Projects/project-name) and add links to them in the `choices` sheet in the `media::image` column.
<table class="xlsTable">
  <thead>
    <tr>
      <th>list_name</th>
      <th>name</th>
      <th>label</th>
      <th>media::image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>animal</td>
      <td>rhino</td>
      <td>Rhino</td>
      <td>rhino.png</td>
    </tr>
    <tr>
      <td>animal</td>
      <td>elephant</td>
      <td>Elephant</td>
      <td>elephant.png</td>
    </tr>
    <tr>
      <td>animal</td>
      <td>lion</td>
      <td>Lion</td>
      <td>lion.png</td>
    </tr>
    <tr>
      <td>animal</td>
      <td>leopard</td>
      <td>Leopard</td>
      <td>leopard.png</td>
    </tr>
    <tr>
      <td>animal</td>
      <td>buffalo</td>
      <td>Buffalo</td>
      <td>buffalo.png</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### 3. Create a `bind::ct:content.style` column
Check out possible values for `style` in the [reference manual]({{ site.baseurl }}/xlsform/reference-manual/4#style).
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### 4. Modify `bind::ct:content.columns` and `bind::ct:content.itemHeight`
It is worth trying out other properties and even modifying the question type to `select_multiple` or `range`.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-3a.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-3b.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-3c.png" /></td>
</tr>
</table>

## Form
[Download XlsForm]({{ site.baseurl }}/assets/xlsform/tutorial-2.xlsx)<br/>

## Demo
