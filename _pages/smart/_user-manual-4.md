## 4. Kiosk mode
Kiosk mode allows SMART Mobile to lock the device so that other phone functions are not accessible. During kiosk mode, users will not be able to exit SMART Mobile to use other applications or phone functions.

The installation process is similar to Android APK mode (see above), however the device must be provisioned. The provisioning process requires that the device be factory reset. 

The APK file for SMART Mobile is available for download from the Download option on the SMART Conservation Tools website: [https://smartconservationtools.org/](https://smartconservationtools.org/Download/SMART-7-Release). 

Limitations:
* Updates will not be automatic. 
* Updates will require repeating the installation process with a new APK. It is not necessary to reprovision the device, the new version can be installed over the old one using the Android APK installation mode (see above).
* Other phone applications cannot be used until first exiting kiosk mode.

### 4.1. Installation
To start, select **Install SMART Mobile on Device…** from the **Field Data** menu and **SMART Mobile** submenu:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image82.png" /></td>
</tr>
</table>

Use the **‘...’** button and select the APK file from the file system and click **Next**:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image102.png" /></td>
</tr>
</table>

Then select **Configure SMART Mobile as a kiosk** and click **Next**:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image228.png" /></td>
</tr>
</table>

Click **Install driver** - once it is installed once, then the button caption will change to **Reinstall driver**. This is a one-time operation on Windows. If the button reads **Reinstall driver**, then there is no need to repeat this process:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image17.png" /></td>
</tr>
</table>

Right click on “android_winusb” (file type: Setup Information) and select **Install**.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image36.png" /></td>
</tr>
</table>

Once the driver is installed, click **Next**.
### 4.2. Preparing the device

If the device is brand new, then there is no need to reset it. Otherwise, factory reset the device by opening **Settings** and selecting **Factory data reset**. Accept all prompts and wait for the device to restart.

Note: it is important to skip creating an account. If an account is active on the device, kiosk mode will not work.

Follow the instructions below and click **Next**:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image241.png" /></td>
</tr>
</table>

Follow the instructions to enable **Developer mode** and **USB debugging** and click **Next**:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image257.png" /></td>
</tr>
</table>

Click **Provision the device** when ready:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image2.png" /></td>
</tr>
</table>

If the process is successful, the following will be shown:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image49.png" /></td>
</tr>
</table>

Other devices may be provisioned directly from here, but plugging them in. When done, click **Finish**.

### 4.3. Desktop configuration
Kiosk mode is configured on a package using Device settings on the SMART Desktop:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/smart/image131.png" /></td>
</tr>
</table>

**Kiosk mode** is a check box. If checked, then launching a Project will activate kiosk mode. Note that this only works if the kiosk version of SMART Mobile is installed.

**Kiosk Mode Exit Pin** controls the pin code needed to exit kiosk mode. When tapping **back** on the start page, the following popup will be displayed:
<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/smart/image130.png" /></td>
</tr>
</table>

Entering the selected code will disable kiosk mode and exit the project.

### 4.4. Field operation
While kiosk mode restricts general use of the device the active project can be changed from the **Settings Page** using **Change project**.
<table>
<tr>
<td><img width="320" src="{{ site.baseurl }}/assets/smart/image13.png" /></td>
</tr>
</table>

From the **Start page**, data can be exported or uploaded. When connected to a Windows PC via USB cable, the data can be downloaded without leaving kiosk mode.
