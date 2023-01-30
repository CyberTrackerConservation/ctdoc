## Header
The header object supports custom header attributes. If no header object is specified, then the default header is used. By default, the header title is taken from the question label.

### color and colorDark
By default, the header background color is taken from the `settings` sheet. However, it is possible to override it on an individual page.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>bind::ct:header.color</th>
      <th>bind::ct:header.colorDark</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one...</td>
      <td>#ff0000</td>
      <td>#800000</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-color-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-color-2.png" /></td>
</tr>
</table>

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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-text.png" /></td>
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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-topText.png" /></td>
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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
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

### homeIcon
Override the home icon with a custom icon.  

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.homeIcon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>my_home_icon.svg</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-homeIcon.png" /></td>
</tr>
</table>

### cancelIcon
When editing a sighting in `immersive` mode, the system puts a **Cancel** button in the top left corner. Clicking this button will discard any edits. This property overrides the default icon used.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.cancelIcon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>my_edit_cancel_icon.svg</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-cancelIcon.png" /></td>
</tr>
</table>

### confirmIcon
When editing a sighting in `immersive` mode, the system puts a **Confirm** button in the top right corner. Clicking this button will accept edits made to the sighting. This property overrides the default icon used.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.confirmIcon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>my_edit_confirm_icon.svg</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-confirmIcon.png" /></td>
</tr>
</table>

### hideHome
If `yes` then the home button is hidden. Default is `no`.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:header.hideHome</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>yes</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

### hidden
If `yes` then the header is hidden. Default is `no`.

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
      <td>no</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-hidden.png" /></td>
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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-header-qml.png" /></td>
</tr>
</table>

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
