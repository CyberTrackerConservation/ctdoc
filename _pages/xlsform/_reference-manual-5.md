## Footer
The footer object supports custom control buttons, e.g. home, back, next, save, etc. If no footer object is specified, then the default control is used.

### buttons
`buttons` is text which specifies which buttons should be shown on the footer toolbar.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.buttons</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one</td>
      <td>animal</td>
      <td>back next index save map</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-buttons-1.png" /></td>
</tr>
</table>

### home button
The `home` button returns to the **Home** page. In `immersive` mode, this returns to the Projects page, otherwise it returns to the project home page.

### back button
The `back` button navigates to the prior question on the form. If the wizard is at the start of the form, the back button is hidden.

### next button
The `next` button navigates to the next question on the form. If there is no next question, then the next button is hidden.

### save button
The `save` button will attempt to save the current sighting. If the sighting has invalid data, then the **Index page** will be shown with invalid fields highlighted.

### nextOrSave button
The `nextOrSave` button will show as a `next` button unless there are no more questions, in which case it will become a `save` button.

### index button
The `index` button displays a list of all the form questions. Selecting a question will navigate the wizard to it directly. A jump-to-last button on the top right of the header will jump to the next required question. If all required questions are filled in, then it jumps to the last question.

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-index-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-index-2.png" /></td>
</tr>
</table>

### options button
The `options` button is only available in `immersive` mode. In non-immersive mode, it becomes the `index` button (see above).

The `options` button shows an options page with two tabs: current sighting and saved sightings:

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-footer-options-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-footer-options-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-footer-options-3.png" /></td>
</tr>
</table>

### map button
The `map` button opens the map dialog.

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-map-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-map-2.png" /></td>
</tr>
</table>

### Custom button icons
The button icons can be overridden with custom ones. To do this, create columns with the name of the button followed by `Icon`. For example:
- homeIcon
- backIcon
- nextIcon
- saveIcon
- indexIcon
- optionsIcon
- mapIcon

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.mapIcon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one</td>
      <td>animal</td>
      <td>my_custom_map_icon.svg</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

### color and colorDark
By default, the footer background color is taken from the `settings` sheet. However, it is possible to override it on an individual page.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>bind::ct:footer.color</th>
      <th>bind::ct:footer.colorDark</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one...</td>
      <td>#0000ff</td>
      <td>#000080</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-color-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-color-2.png" /></td>
</tr>
</table>

### buttonColor and buttonColorDark
Override the default button color with a custom one. This applies to all buttons.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>bind::ct:footer.buttonColor</th>
      <th>bind::ct:footer.buttonColorDark</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one...</td>
      <td>#00a000</td>
      <td>#20f020</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-buttonColor-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-buttonColor-2.png" /></td>
</tr>
</table>

### buttonScale
An additional scaling factor to apply to the button size. This is typically useful for increasing the size of footer buttons. The scaling factor will be capped to allow at least 6 buttons to fit in the footer.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>bind::ct:footer.buttonScale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one...</td>
      <td>3.5</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-buttonScale.png" /></td>
</tr>
</table>

### hidden
If `yes` then the footer is hidden. Default is `no`.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.hidden</th>
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

### qml
A [QML](https://wikipedia.org/wiki/QML) fragment to use instead of the built-in footer. See Developer section. For example: 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.qml</th>
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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

To set the footer to a blue rectangle, replace `qml fragment` above with the following:
```qml
import QtQuick 2.15

Rectangle {
    color: "blue"
    height: 64
}
```

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-footer-qml.png" /></td>
</tr>
</table>

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
