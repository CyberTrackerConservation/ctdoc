## 5. Retrieving data
Once data has been entered, use the **Export data** button on the project home page to ready the process. For Collect, click on the **Upload data** button to complete data upload.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image42.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image55.png" /></td>
</tr>
</table>

### 5.1. USB cable
Connect the USB cable from the desktop to the device. Ensure the device is in **File Transfer** mode.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image173.png" /></td>
</tr>
</table>

When correctly configured, the device will be present in **Windows Explorer**:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image45.png" /></td>
</tr>
</table>

Choose **Import…** from the **Field Data -> SMART Mobile** menu.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image44.png" /></td>
</tr>
</table>

This will open the **Import SMART Mobile Data dialog**. Select **Device** and then click **Import**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image4.png" /></td>
</tr>
</table>

### 5.2. Connect
When SMART is configured with a Connect server, it can be configured to send data automatically. If **Upload Data To Connect** is unchecked, then data must be retrieved using the **USB cable** (see above). Otherwise, it will be sent directly to the Connect server over the network.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image124.png" /></td>
</tr>
</table>

Since the connection to the server may be interrupted, the **Export data** option will attempt to send all unsent data to the server.

### 5.3. Collect
Collect automatically sends data to the server. After collection has completed, the **Upload data** button becomes visible. This sends any unsent data and resets the project.
