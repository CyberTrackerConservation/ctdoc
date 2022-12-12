## Save
When the user presses the Save button, this triggers the save behavior.

### snapLocation

Setting `snapLocation` to true will create a popup to acquire the GPS location. The location will be set in the first `geopoint` type question on the form. It is recommended to set the `hidden` column on this question, so that the user is not asked for the location beforehand.  

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save.snapLocation</th>
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

### targets
In the example below, the user will be presented with a popup containing the choices **Restart** or **Continue**. Depending on which is selected, a new sighting will be created starting at the targetted question.

`restart` and `continue` are taken from the `choices` sheet in the `saveTargets` list name.

`question` is the name of the targetted question in the `survey` table. If the question is not relevant, then this choice will be ignored.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save.targets</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>[{ "choice": "restart", "question": "animal"}, { "choice": "continue", "question": "count"}]</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

<table class="xlsTable">
  <thead>
    <tr>
      <th>list_name</th>
      <th>name</th>
      <th>label</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>saveTarget</td>
      <td>restart</td>
      <td>Restart</td>
    </tr>
    <tr>
      <td>saveTarget</td>
      <td>continue</td>
      <td>Continue</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

### track
In the example below, there is a `select_one` question called `start_stop` with choices `start` and `stop`. When the user presses **Save**, the track timer is adjusted depending on which choice was selected. The values in `updateIntervalSeconds` and `distanceFilterMeters` are the new track settings.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>bind::ct:save.track</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>integer</td>
      <td>animal_count</td>
      <td>[{ "condition": "${start_stop}='start'", "updateIntervalSeconds": 5, "distanceFilterMeters": 120 }, { "condition": "${start_stop}='stop'", "updateIntervalSeconds": 0, "snapTrack": true }]</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>survey</span></td>
    </tr>
  </tfoot>
</table>

`condition` is an XlsForm expression which activates this option if matched, e.g. ${start_stop}='start'. Check out the [ODK Form Logic documentation](https://docs.getodk.org/form-logic/).

`updateIntervalSeconds` is the number of seconds between GPS readings. Set to 0 to disable the track timer.

`distanceFilterMeters` is the minimum distance between readings in meters. This is optional and by default no distance filter is used.

`snapTrack` causes the system to snapshot all the track points (since prior snap). If using the Survey123 provider and  `bind::ct:esriLocationServiceUrl` is specified, then the track data will be sent to the feature service. Otherwise, a track file will be created and added to a `file` type question in the form. The question selected must be of type `file` and should have a `trackFileFormat` column specified.
