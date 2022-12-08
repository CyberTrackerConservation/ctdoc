## Initial setup

These columns on the `settings` sheet are needed to begin using the CyberTracker extensions. 

### namespace (required)
The `ct` namespace tells other XlsForm tools to ignore columns starting with `bind::ct:`.
<table class="xlsTable">
  <thead>
    <tr>
      <th>title</th>
      <th>version</th>
      <th>namespaces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>My Form</td>
      <td>2022101001</td>
      <td>ct="http://cybertracker.org/xforms"</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td class="sheets" colspan="3"><span>survey</span><span>choices</span><span class="active">settings</span></td>      
    </tr>
  </tfoot>
</table>

### version (recommended)
The version field is used to track form versions as they change over time. While it is not required, it is a best practice to keep this field up to date. The [XlsForm specification](https://xlsform.org/#settings-worksheet) recommends the convention like 'yyyymmddrr'. For example, 2022021501 is the 1st revision from Feb 15th, 2022.