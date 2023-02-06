## Save
When the user presses the **Save** button, this triggers the save behavior.

### snapLocation

Setting `snapLocation` to the name of a `geopoint` question will create a popup to acquire the GPS location. This feature is only active when `wizardMode` is enabled.

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
      <td>geopoint</td>
      <td>f_location</td>
      <td>Location</td>
    </tr>
    <tr>
      <td>select_one animal</td>
      <td>f_animal</td>
      <td>Animal</td>
    </tr>
    <tr>
      <td>text</td>
      <td>f_note</td>
      <td>Note</td>
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
      <th>bind::ct:save.snapLocation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My form</td>
      <td>f_location</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>

In this example, the user flow will be:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-snapLocation-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-snapLocation-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-snapLocation-3.png" /></td>
</tr>
</table>

### targets
In the example below, the user will be presented with a popup containing the choices **Restart** or **Another**. After the sighting is saved, a new sighting will be created starting at the targeted question. All prior question data will be replicated into the new sighting.

This value must be a valid JSON array.

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
      <td>f_note</td>
      <td>Note</td>
    </tr>        
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span class="active">survey</span><span>choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

`restart` and `another` are taken from the `choices` sheet in the `saveTargets` list name.

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
      <td>another</td>
      <td>Another</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

Note that `question` is the name of the targeted question in the `survey` table. If the question is not relevant, then this choice will be hidden.

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:save.targets</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My form</td>
      <td>[{ "choice": "restart", "question": "f_animal"}, { "choice": "another", "question": "f_behavior"}]</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>

Note that if `immersive` is set to false, then the target list will automatically contain the **home** button. This option will save and return to the **Home** page without automatically creating a new sighting.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTarget-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTarget-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTarget-3.png" /></td>
</tr>
</table>

### track
In the example below, there is a `select_one` question called `f_track` with choices `start`, `stop` and `nochange`. When the user presses **Save**, the track timer is adjusted depending on which choice was selected. The values in `updateIntervalSeconds` and `distanceFilterMeters` are the new track settings.

This value must be a valid JSON array.

<table class="xlsTable">
  <thead>
    <tr>
      <th>type</th>
      <th>name</th>
      <th>label</th>
      <th>appearance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>file</td>
      <td>f_track_file</td>
      <td>Track file</td>
      <td>hidden</td>
    </tr>
    <tr>
      <td>select_one track_items</td>
      <td>f_track</td>
      <td>Configure track</td>
      <td></td>
    </tr>
    <tr>
      <td>text</td>
      <td>f_note</td>
      <td>Note</td>
      <td></td>
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
      <th>list_name</th>
      <th>name</th>
      <th>label</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>track_items</td>
      <td>start</td>
      <td>Start</td>
    </tr>
    <tr>
      <td>track_items</td>
      <td>stop</td>
      <td>Stop</td>
    </tr>
    <tr>
      <td>track_items</td>
      <td>nochange</td>
      <td>No change</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span class="active">choices</span><span>settings</span></td>
    </tr>
  </tfoot>
</table>

<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>bind::ct:save.trackFile</th>
      <th>bind::ct:save.track</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My form</td>
      <td>f_track_file</td>
      <td>[{ "condition": "selected(${f_track}, 'start')", "updateIntervalSeconds": 5, "distanceFilterMeters": 10 }, { "condition": "selected(${f_track},'stop')", "updateIntervalSeconds": 0, "snapTrack": true }]</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>
    </tr>
  </tfoot>
</table>

`condition` is an XlsForm expression which activates this option if matched, e.g. ${start_stop}='start'. Check out the [ODK Form Logic documentation](https://docs.getodk.org/form-logic/).

`updateIntervalSeconds` is the number of seconds between GPS readings. Set to 0 to disable the track timer.

`distanceFilterMeters` is the minimum distance between readings in meters. This is optional and by default no distance filter is used.

`snapTrack` causes the system to snapshot all the track points (since prior snap). 

If using Survey123 and `esriLocationServiceUrl` is specified, then the track data will be sent to the [feature service]({{ site.baseurl }}/xlsform/reference-manual/2#esrilocationserviceurl). Otherwise, a track file will be created and added to a `file` type question in the form. See the section on the track file [here]({{ site.baseurl }}/xlsform/reference-manual/#track-file-format).

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-3.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-5.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-saveTrack-6.png" /></td>
</tr>
</table>
