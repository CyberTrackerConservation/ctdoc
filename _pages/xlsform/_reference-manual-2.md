## Settings

### immersive
Setting this to `true` causes the UI to use the wizard exclusively, i.e. there is no **Home** page. Default is `false`. `TRUE` and `FALSE` values also work.
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
      <td>true</td>
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
If the `immersive` column is missing or set to `false`, then the UI reverts to *non-immersive* mode. In this case, there is a **Home** page which shows all sightings. The user returns to this page after saving a sighting. 

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:immersive</th>
      <th>bind::ct:wizardMode</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>false</td>
      <td>true</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

If `wizardMode` is set to `false`, then all questions show on a single page. This mode is recommended when wanting to show all sighting data at once and is the most conventional. 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-3.png" /></td>
</tr>
</table>

If `wizardMode` is set to `true`, then each question will appear on its own page with **Back** and **Next** toolbar buttons to navigate between questions. The user will still return to the **Home** page between sightings. wizardMode appears on the **Settings** page as **Page mode**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-5.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-wizardMode-6.png" /></td>
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
- primary
- accent
- foreground
- background
- darkPrimary
- darkAccent
- darkForeground
- darkBackground

Colors prefixed with 'dark' will be used when dark mode is activated. If dark colors are not provided, then 'primary' and 'accent' colors will be used, but 'foreground' and 'background' colors will be ignored.

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

If this service is not specified, then tracks are placed in a `file` type question of the sighting which specifies `snapTrack` in the `save` section of the `survey` question. See [Tracks]({{ site.baseurl }}/xlsform/reference-manual/6#track).

### sendLocationInterval

If using Survey123, CyberTracker can send the current location at regular intervals - separately from tracks. The value is in seconds and is user configurable via the form Settings menu on the device. This specifies the default value. `bind::ct:esriLocationServiceUrl` must be configured.

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
