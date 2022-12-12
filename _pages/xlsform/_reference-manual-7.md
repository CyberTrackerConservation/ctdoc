## Miscellaneous

### fixCount
For `geopoint` question types, the number of skipped readings before a fix is taken. The default value is 4.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:fixCount</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geopoint</td>
      <td>my_location</td>
      <td>4</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### trackFileFormat
When the user presses **Save** and creates a track file, it is stored in a `file` field which has the `trackFileFormat` value set.

Supported values are `kmz` (not supported on Survey123) and `geojson` (inside a zip). 

Survey123 users should prefer to use a location service - see `esriLocationServiceUrl` in the `settings` sheet. If a location service is specified, this question should be removed.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>appearance</th>
      <th>bind::ct:trackFormat</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>file</td>
      <td>my_track_file</td>
      <td>hidden</td>
      <td>kmz</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>
