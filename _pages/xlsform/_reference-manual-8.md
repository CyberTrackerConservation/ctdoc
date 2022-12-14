## Developers

### Introduction
CyberTracker is built on the [Qt Framework](https://www.qt.io/product/framework). The Qt user-interface language is called [QML](https://en.wikipedia.org/wiki/QML) and it provides a concise way to describe components and layouts. The scripting language is Javascript.

QML fragments can be added to an XlsForm. This enables a high degree of customization beyond what is already available. In particular it allows custom widgets and layouts to be used in data entry.

### Setup
Install CyberTracker on your desktop computer by following the instructions on the [Download page]({{ site.baseurl }}/xlsform/download).

After launching, open the **Window** menu and select **Toggle developer console**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-dev-0.png" /></td>
</tr>
</table>

### Page layout
Each question in an XlsForm is given one page in the UI. The page is divided into 3 segments: header, content and footer:
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-dev-1.png" /></td>
</tr>
</table>

Each can host QML and these are specified in the `bind::ct:header.qml`, `bind::ct:content.qml` and `bind::ct:footer.qml` columns. Note that you may also use `qmlFile` (file alongside project files) or `qmlBase64` (base64 encoded QML).

### recordUid and fieldUid
XlsForm question values are identified by their `recordUid` and `fieldUid`. 

`recordUid` uniquely identifies the current record. For simple forms there is only record per sighting, but using [repeats](https://xlsform.org/#repeats) and groups, multiple records will be created.

`fieldUid` uniquely identifies the question within a form. It comes from the `name` column of the `survey` sheet.

Given the following form:
<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:content.qmlFile</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>text</td>
      <td>my_field_name</td>
      <td>My field name</td>
      <td>test.qml</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

And the following test.qml:
```qml
import QtQuick 2.15

Item {
    property string recordUid
    property string fieldUid

    Component.onCompleted: {
        console.log("recordUid = " + recordUid)
        console.log("fieldUid = " + fieldUid)
    }
}
```

The developer console will output something like:
```
recordUid = 7f1ed933401b43878fee6f0d38c7f92a
fieldUid = my_field_name
```

### Setting form values
Form values can be changed using a FieldBinding component. This enables change notifications so that the Label will automatically update when the button is clicked.
```qml
import QtQuick 2.15
import QtQuick.Controls 2.15
import CyberTracker 1.0 as C

Item {
    property alias recordUid: fieldBinding.recordUid
    property alias fieldUid: fieldBinding.fieldUid

    C.FieldBinding {
        id: fieldBinding
    }

    Label {
        x: 10
        y: 10
        text: fieldBinding.value
    }

    Button {
        anchors.centerIn: parent
        text: "Set field value"
        onClicked: {
            fieldBinding.setValue("Hello world!")
        }
    }
}
```
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-dev-2.png" /></td>
</tr>
</table>

The console window will give an error of the form: `Unable to assign [undefined] to QString` when first launched, because `fieldBinding.value` is initially undefined. This is generally harmless, but can be removed by checking for undefined:
```qml
Label {
    x: 10
    y: 10
    text: fieldBinding.value || ""
}
```