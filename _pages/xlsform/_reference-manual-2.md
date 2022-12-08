## Settings

### immersive
Setting this to `true` causes the form UI to use the wizard exclusively, i.e. this is more like CyberTracker Classic. Default is `false`. `TRUE` and `FALSE` values also work.
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

When using Survey123, CyberTracker supports uploading locations and tracks to a hosted feature service. In this case, the feature service is specified in the esriLocationServiceUrl column:

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

The feature service contains three layers: Tracks (point layer), Last Known Locations (point layer) and Track Lines (Polyline layer). 

If this service is not specified, then tracks are placed in a `file` type question of the sighting which specifies `snapTrack` in the `save` section of the `survey` question. 

### sendLocationInterval

CyberTracker can send the current location at regular intervals, separately from a the track system. This value is in seconds and is user configurable - this specifies the default value. For Survey123, `esriLocationServiceUrl` must be configured.

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
