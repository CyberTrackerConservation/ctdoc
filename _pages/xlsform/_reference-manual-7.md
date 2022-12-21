## Miscellaneous

### fixCount
For `geopoint` question types, the number of skipped readings before a fix is taken. The default value is 4. Some GPS devices return old readings before real readings. To overcome this, setting the `fixCount` will cause the system to require several readings before the final location is taken. 

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>geopoint</td>
      <td>f_location</td>
      <td>fixCount=4</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

### track file format
When the user presses **Save** and creates a track file, it is stored in a `file` field specified in the `settings` sheet in the `bind::ct:save.trackFile` column. 

By default the format of the track is zipped geojson, but this can be changed by using the `format` parameter of the question itself. Supported values are `geojson` and `kmz` (not supported on Survey123). 

Survey123 users should prefer to use a location service - see [esriLocationServiceUrl]({{ site.baseurl }}/xlsform/reference-manual/2#esrilocationserviceurl). If a location service is specified, this question should be removed.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>appearance</th>
      <th>parameters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>file</td>
      <td>f_track_file</td>
      <td>hidden</td>
      <td>format=kmz</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:save.trackFile</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My form</td>
      <td>f_track_file</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>
