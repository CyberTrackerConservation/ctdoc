## Content
The content section is the middle part of the screen between the header and footer. By default it automatically selects a control for the question type, e.g. a date selector for a date question. By specifying a custom content object, more styles are available. This is especially useful for customizing lists.

### frameWidth
Frame width around the content area of the page. Default is 16.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.frameWidth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>16</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### style 
The visual appearance of the question. 

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

For **select_one** questions
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

### padding
The padding space between grid items. Requires `style` to be set.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.padding</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>4</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### columns
Number of columns for grids. Requires `style` to be set. Defaults to 2.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.columns</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>4</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### lines
Show lines between cells for grids. Requires `style` to be set. Defaults to true.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.lines</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>false</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### border
Show border around the outside of a grid. Requires `style` to be set. Defaults to false if contentPadding is 0, true otherwise.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.border</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### borderWidth
Border width for grid lines. Requires `style` to be set. Defaults to 2.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.borderWidth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>3</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### fontSize
Size text font size. Requires `style` to be set. Defaults to 16.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.fontSize</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>14</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### fontBold
Set font to bold. Requires `style` to be set. Defaults to false.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.fontBold</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### itemHeight
Set height of individual items. Requires `style` to be set. Defaults to 48.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.itemHeight</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>64</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### qml
A [QML](https://wikipedia.org/wiki/QML) fragment to use instead of the built-in content. See Developer section. For example: 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.qml</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>qml fragment</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

To set the content to a blue rectangle, replace `qml fragment` above with the following:
```qml
import QtQuick 2.15

Rectangle {
    color: "blue"
}
```

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
