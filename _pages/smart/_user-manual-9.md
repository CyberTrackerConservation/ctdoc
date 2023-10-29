## 9. Troubleshooting
### 9.1. Creating a bug report

When reporting an error or unexpected condition, a bug report is essential. When asked to create one, go to the main **Settings** tab and scroll to the bottom:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image157.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image168.png" /></td>
</tr>
</table>

**Share bug report** requires that the device has a network connection. The bug report will be created and sent to the device sharing system. This allows sending over various channels like email, Whatsapp, etc. The report can also be beamed to another device via NFC or Bluetooth.

**Save bug report** is only available on Android. This saves the report to a file on the device and it can then be retrieved using a USB cable.

Bug reports contain a full copy of the SMART Mobile data on the device. This includes confidential information such as the access to Connect servers and even old data. They should therefore be handled carefully.

### 9.2. Recovering Exported data
SMART data is exported to JSON files. If the normal import operation is not functioning, then it is possible to retrieve the JSON files from the device and import them manually. To do this, go to the **Settings** page and tap **Exported data**. Then tap the file to retrieve and the **Share** button. This will open the sharing options for the device. Send the file through another channel and copy it to the SMART Desktop computer.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image99.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image90.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image35.png" /></td>
</tr>
</table>

Open the **Import SMART Mobile Data** dialog, **Add** the file and click **Import**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image50.png" /></td>
</tr>
</table>


### 9.3. Recovering Connect data
If SMART Mobile is configured to send data to SMART Connect and the Connect server is not available, outstanding data can be recovered using the **Recover Connect data** option off the **Settings** page. All the data that would ordinarily have been sent to Connect is exported to a file. This can then be downloaded over USB cable or shared using another channel (see **Recovering Exported Data** above).
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image79.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image133.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/image1.png" /></td>
</tr>
</table>

### 9.4. Waiting for time correction
When the device is first used, the message **Waiting for time correction** may appear. This is a one time operation where SMART Mobile is calibrating the device clock to ensure that the time is correct.

If this is taking a long time, try taking the device into an open area to make sure that the GPS has a good reading.

### 9.5. Android device data
If importing the data from the device is not working, it is possible to retrieve exported data directly from the device.

Connect the device to Windows and set the **USB mode** to **File transfer**.

Open Windows Explorer and navigate to the folder:

**\Android\data\org.cybertracker.mobile.smk\files\SMARTdata**

This folder contains the JSON data files.

### 9.6. Blackview track logging 
Some Blackview devices try to prevent background tasks from using the battery. The symptoms of this issue are that track logging is disabled after 10 minutes.

To solve this, Blackview has provided a **System Manager** application which allows applications to be excluded from this behavior. The steps are:
1. Run the `System Manager` application
1. Select `App Management`
1. Select `Auto cleanup`
1. Scroll down to `SMART Mobile` and enable the switch to prevent cleanup

If the below user experience does not match your device, check out [Don't kill by app](https://dontkillmyapp.com/blackview).
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/blackview-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/blackview-2.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/blackview-3.png" /></td>
<td><img src="{{ site.baseurl }}/assets/smart/blackview-4.png" /></td>
</tr>
</table>
