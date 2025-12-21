---
layout: page
title: Get exported data
parent: SMART Mobile
permalink: /smart/get-exported-data/
---
# Get exported data

The normal way to retrieve data from SMART Mobile over USB is to import the data using the **Field data -> SMART Mobile -> Import data** menu option.

This recently stopped working due to mobile security changes.

This is the work around.

1. Install SMART Mobile build 585 or later. It is available on the Google Play Store or you can get the APK from [here]({{ site.baseurl }}/smart/download).
1. Connect the USB cable and select **File Transfer** mode on the device
1. Open Windows Explorer, select your device and navigate to the **Download** folder and then the **SMARTdata** folder
1. Copy the JSON files there to any desktop folder (or create a new one)
1. Use the **Field data -> SMART Mobile -> Import data** menu option and set **Import From** to **Files**
1. Use the **Add** button to select the files you copied and then click **Open**
1. Once you have confirmed the data was imported, delete the JSON files from your desktop
1. Delete the files from the SMARTdata folder on the device
