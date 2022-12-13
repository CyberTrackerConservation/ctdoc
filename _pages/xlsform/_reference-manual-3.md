## Header
The header object supports custom header attributes. If no header object is specified, then the default header is used. By default, the header title is taken from the question label.

### text
Custom header text.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.text</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>Animal</td>
      <td>Custom question text</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/xlsform/refman-header-text.png" /></td>
</tr>
</table>

### topText
Custom smaller text above main title.
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.topText</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>Custom top text</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/xlsform/refman-header-topText.png" /></td>
</tr>
</table>

### button
Type of the button in the top-right corner. Valid values are:
- empty - by default no button is shown
- `track` - the current state of the GPS track system
- `battery` - the current state and level of the battery 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.button</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>track</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

Tapping on the button will provide more information, e.g. the track frequency or the battery level.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-header-button-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-header-button-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-header-button-3.png" /></td>
</tr>
</table>

### hidden
If `true` then the header is hidden. Default is `false`.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.hidden</th>
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

<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/xlsform/refman-header-hidden.png" /></td>
</tr>
</table>

### qml
A [QML](https://wikipedia.org/wiki/QML) fragment to use instead of the built-in header. See Developer section. For example: 

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
      <td>select_one animal</td>
      <td>animal</td>
      <td>qml fragment</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

To set the header to a blue rectangle, replace `qml fragment` above with the following:
```qml
import QtQuick 2.15

Rectangle {
    color: "blue"
    height: 64
}
```

<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/xlsform/refman-header-qml.png" /></td>
</tr>
</table>

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
