## Settings

### immersive
Setting this to `yes` causes the UI to use the wizard exclusively, i.e. there is no **Home** page. Default is `no`.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:immersive</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>yes</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

In the table below, the user context is always within a sighting and each page typically holds one question. Pressing the **options** button (highlighted in the first image) navigates to a new page which shows the current sighting on one tab and all sightings on the other. The user can edit previous sightings, but when editing is complete, the wizard will revert to the original sighting.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-immersive-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-immersive-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-immersive-3.png" /></td>
</tr>
</table>

### wizardMode
If the `immersive` column is missing or set to `no`, then the UI reverts to *non-immersive* mode. In this case, there is a **Home** page which shows all sightings. The user returns to this page after saving a sighting. 

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:wizardMode</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>yes</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

If `wizardMode` is set to `no`, then all questions show on a single page. This mode is recommended when wanting to show all sighting data at once and is the most conventional. 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-3.png" /></td>
</tr>
</table>

If `wizardMode` is set to `yes`, then each question will appear on its own page with **Back** and **Next** toolbar buttons to navigate between questions. The user will still return to the **Home** page between sightings. wizardMode appears on the **Settings** page as **Page mode**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-5.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-6.png" /></td>
</tr>
</table>

### summaryText and summaryIcon
The summary attribute specifies which fields to use as the summary of a sighting on the **Home** page. For example:

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>text</td>
      <td>f_initial_text</td>
      <td>Initial note</td>
    </tr>
    <tr>
      <td>select_one animal</td>
      <td>f_animal</td>
      <td>Animal</td>
    </tr>
    <tr>
      <td>select_multiple behavior</td>
      <td>f_behavior</td>
      <td>Behavior</td>
    </tr>
    <tr>
      <td>text</td>
      <td>f_final_text</td>
      <td>Final note</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

The following setting will ensure that the summary text only uses the `f_animal` and `f_behavior` questions. Similarly, the summary icon will be taken from the `f_animal` question.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:summaryText</th>
      <th>bind::ct:summaryIcon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>f_animal f_behavior</td>
      <td>f_animal</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-setting-summary-1.png" /></td>
</tr>
</table>

### colors
The colors attribute specifies the color scheme used on the form. It follows the [Material Design](https://m2.material.io/design/color/the-color-system.html) system:
<br/><img src="{{ site.baseurl }}/assets/xlsform/material_design.png" />

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:colors.primary</th>
      <th>bind::ct:colors.accent</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>#6200EE</td>
      <td>green</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

The following color fields are supported:
- primary & primaryDark
- accent & accentDark
- foreground & foregroundDark
- background & backgroundDark

Colors suffixed with 'dark' will be used when dark mode is activated. If dark colors are not provided, then 'primary' and 'accent' colors will be used, but 'foreground' and 'background' colors will be ignored.

Colors can also be provided as a JSON object:

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:colors</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>{ "primary": "#6200EE", "accent": "green" }</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### icon, iconDark and subtitle
The `icon` attribute specifies the icon used to display the project. `iconDark` is optional and will used when dark mode is enabled.

The `subtitle` attribute specifies the text just below the form name. 

<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-setting-icon-subtitle.png" /></td>
</tr>
</table>

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:icon</th>
      <th>bind::ct:subtitle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>gorilla.png</td>
      <td>Custom subtitle</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

The icon image should be added to the form as an attached media file. In KoBoToolbox, this is done under the form settings option:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-setting-icon-kobo.png" /></td>
</tr>
</table>

### offlineMapUrl

The `offlineMapUrl` attribute specifies a url to a downloadable zip file containing map layers. Offline maps can be added manually using the mobile app, but this provides a way to specify them with the form. The map will be downloaded, installed and updated as part of the form.

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:offlineMapUrl</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>https://cybertrackerwiki.org/assets/xlsform/offlinemap.zip</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

See the section on [Offline maps]({{ site.baseurl }}/xlsform/reference-manual/maps) for more information.

### esriLocationServiceUrl

When using Survey123, CyberTracker supports uploading locations and tracks to a hosted feature service. In this case, the feature service is specified in the `bind::ct:esriLocationServiceUrl` column:

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:esriLocationServiceUrl</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>https://services6.arcgis.com/.../FeatureServer</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

The feature service should be created using the CyberTracker Desktop Simulator (see [Download page]({{ site.baseurl }}/xlsform/download)). There is an option off the **Tools** menu called **Create ArcGIS location service**. This tool will automatically create and configure a hosted service which is compatible with CyberTracker:

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-esri-1.png" /></td>
</tr>
</table>

After clicking **Start**, the tool will display the following:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-esri-2.png" /></td>
</tr>
</table>

The feature service contains three layers: **Tracks** (point layer), **Last Known Locations** (point layer) and **Track Lines** (Polyline layer). 

If this service is not specified, then tracks are placed in a `file` type question of the sighting. See [Tracks]({{ site.baseurl }}/xlsform/reference-manual/6#track).

### sendLocationInterval

If using Survey123, CyberTracker can send the current location at regular intervals - separately from tracks. The value is in seconds and is user configurable via the form Settings page on the device. This specifies the default value. `bind::ct:esriLocationServiceUrl` must be configured.

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:sendLocationInterval</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>30</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### submitInterval

Auto-submit at a timer interval. The value is in seconds and is user configurable via the form Settings page on the device. It is equivalent to manually pressing the Submit button. The default value is `0` meaning auto-submission is disabled. A value of `1` means that submit is combined with the save operation.

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:submitInterval</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>300</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>
