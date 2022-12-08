## Footer
The footer object supports custom control buttons, e.g. back, next, save, etc. If no footer object is specified, then the default control is used.

### options
Show **options** button in immersive mode. Show **index** button in non-immersive mode. Default is true.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.options</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### map
Show **map** button. Default is true.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.map</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>false</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### save
Show save button. Default is false.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.save</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### next
Show next button. Default is true, if there is a next page.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:footer.next</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>false</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### hidden
If `true` then the footer is hidden. Default is `false`.

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
      <td>integer</td>
      <td>animal_count</td>
      <td>false</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
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

To set the footer to a blue rectangle, replace `qml fragment` above with the following:
```qml
import QtQuick 2.15

Rectangle {
    color: "blue"
    height: 64
}
```

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
