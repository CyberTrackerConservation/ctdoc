## Content
The content section is the middle part of the screen between the header and footer. By default it automatically selects a control for the question type, e.g. a date selector for a date question. By specifying a custom content object, more styles are available. This is especially useful for customizing lists.

### color and colorDark
By default, the content background color is taken from the `settings` sheet. However, it is possible to override it on an individual page.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>bind::ct:content.color</th>
      <th>bind::ct:content.colorDark</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one...</td>
      <td>#a0b0c0</td>
      <td>#102030</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-color-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-color-2.png" /></td>
</tr>
</table>

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
      <td>select_one animal</td>
      <td>animal</td>
      <td>0</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

In this case, `frameWidth` was set to `0` in the second image. 
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-frameWidth-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-frameWidth-2.png" /></td>
</tr>
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
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

For **select_one** questions
- (not specified)
- IconOnly
- TextOnly
- TextBesideIcon
- TextUnderIcon

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-3.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-5.png" /></td>
</tr>
</table>

For **select_multiple** questions:
- (not specified)
- IconInlay
- IconOnly
- TextOnly
- TextBesideIcon

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-7.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-8.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-9.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-10.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-style-11.png" /></td>
</tr>
</table>

For **number list** groups:
- (not specified)
- IconOnly
- TextOnly
- TextBesideIcon

Number lists are a set of questions inside a `group`. The `appearance` column must be set to `field-list` to force all group questions to appear on the same page: 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:content.style</th>
      <th>appearance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>begin group</td>
      <td>numberlist</td>
      <td>Number list</td>
      <td>IconOnly</td>
      <td>field-list</td>
    </tr>
    <tr>
      <td>integer</td>
      <td>number1</td>
      <td>Number 1</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>integer</td>
      <td>number2</td>
      <td>Number 2</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>integer</td>
      <td>number3</td>
      <td>Number 3</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>integer</td>
      <td>number4</td>
      <td>Number 3</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>integer</td>
      <td>number5</td>
      <td>Number 5</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>end group</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-numberlist-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-numberlist-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-numberlist-3.png" /></td>
</tr>
</table>

For **range** questions:

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>parameters</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.columns</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>range</td>
      <td>animal_count</td>
      <td>start=1 end=100 step=1</td>
      <td>Grid</td>
      <td>5</td>
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
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-range-1.png" /></td>
</tr>
</table>

For a fixed number of **image** questions:

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:content.style</th>
      <th>appearance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>begin group</td>
      <td>photogroup</td>
      <td>Group photos</td>
      <td>Grid</td>
      <td>field-list</td>
    </tr>
    <tr>
      <td>image</td>
      <td>image1</td>
      <td>Photo</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>image</td>
      <td>image2</td>
      <td>Photo 2</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>image</td>
      <td>image3</td>
      <td>Photo 3</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>image</td>
      <td>image4</td>
      <td>Photo 4</td>
      <td></td>
      <td></td>
    </tr>    
    <tr>
      <td>end group</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogroup-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogroup-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogroup-3.png" /></td>
</tr>
</table>

For a dynamic number of **image** questions:

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>bind::ct:content.style</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>begin repeat</td>
      <td>photogroup</td>
      <td>Repeat photos</td>
      <td>Grid</td>
    </tr>
    <tr>
      <td>image</td>
      <td>image</td>
      <td>Photo</td>
      <td></td>
    </tr>    
    <tr>
      <td>end repeat</td>
      <td></td>
      <td></td>
      <td></td>
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
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogrid-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogrid-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-photogrid-3.png" /></td>
</tr>
</table>

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
      <td>8</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

Padding values are `0`, `4` and `8`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-padding-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-padding-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-padding-3.png" /></td>
</tr>
</table>

### columns
Number of columns for grids. Requires `style` to be set. Defaults to 2.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.columns</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>Grid</td>
      <td>4</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

For example, column values below are `3`, `5` and `10`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-columns-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-columns-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-columns-3.png" /></td>
</tr>
</table>

### lines
Show lines between cells for grids. Requires `style` to be set. Defaults to true.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.lines</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>no</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

`lines` value below is `yes` and `no`.
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-lines-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-lines-2.png" /></td>
</tr>
</table>

### border
Show border around the outside of a grid. Requires `style` to be set. Defaults to `no` if frameWidth is 0, `yes` otherwise.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.border</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>yes</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

Border value is `yes` and `no`.
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-border-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-border-2.png" /></td>
</tr>
</table>

### borderWidth
Border width for grid lines. Requires `style` to be set. Defaults to 2.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.borderWidth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

borderWidth value is `2` and `4`.
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-borderWidth-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-borderWidth-2.png" /></td>
</tr>
</table>

### fontSize
Size text font size. Requires `style` to be set. Defaults to 16. Note that the font is subject to scaling according to the **Font size** in the main Settings page.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.fontSize</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>14</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

`fontSize` values are `10`, `14` and `18`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-fontSize-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-fontSize-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-fontSize-3.png" /></td>
</tr>
</table>

### fontBold
Set font to bold. Requires `style` to be set. Defaults to false.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.fontBold</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>yes</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
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
      <th>bind::ct:content.style</th>
      <th>bind::ct:content.itemHeight</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>select_one animal</td>
      <td>animal</td>
      <td>IconOnly</td>
      <td>48</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

`itemHeight` values are `48`, `64` and `128`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-itemHeight-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-itemHeight-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-content-itemHeight-3.png" /></td>
</tr>
</table>

### qml
A [QML](https://wikipedia.org/wiki/QML) fragment to use instead of the built-in content. See Developer section. For example: 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:content.qml</th>
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

To set the content to a blue rectangle, replace `qml fragment` above with the following:
```qml
import QtQuick 2.15
import QtQuick.Controls 2.15

Rectangle {
    color: "blue"
    Button {
        anchors.centerIn: parent
        text: "Click me"
        onClicked: parent.color = "red"
    }
}
```

In the example, the content is blue, then changes to red when the button is clicked.
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-qml-1.png" /></td>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-content-qml-2.png" /></td>
</tr>
</table>

### qmlBase64
Base64 encoded QML (see **qml** above).

### qmlFile
Name of a QML file which exists alongside other project files. This is not supported on ODK or KoBoToolbox, but can be used in Survey123.
