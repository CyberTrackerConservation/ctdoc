### Kiosk mode

Kiosk mode is a function which locks your device to the function of a specific application and prevents the use of any other application. Essentially, using kiosk mode will turn your device into a SMART-Mobile-Only device.

#### When to use kiosk mode

Deciding whether to use kiosk mode is highly dependent on your
particular use case. If you feel it is necessary to lock a device to
SMART Mobile only then kiosk mode is for you. This might be to ensure
that devices procured for SMART data collection are used only for this
function and nothing else. By dedicating your mobile device for SMART
mobile data collection, kiosk mode simplifies data collection, focuses
attention on that task alone, and conserves device resources.

#### When not to use kiosk mode

If you or your field team need to use other functionality on data
collection devices, then kiosk mode is *not* required. Other apps that
may be used in the field include telephone function or communication
applications, additional navigation applications, specific camera
applications, and others (note: SMART Mobile does record track data and
images). If your field teams do not need these other applications, then
you may want to consider using kiosk mode.

### How to enable kiosk mode

Once you have made a decision about whether or not to use kiosk mode,
you must make a change in the SMART Conservation Area (CA) on your
computer in the settings for your configurable model.

Login into your SMART CA then go to Conservation Area \> Configurable
Model.

- Select the model you wish to use from the list
![]({{ site.baseurl }}/assets/smart/image199.png)
- Select **Edit** and go to the **CyberTracker** properties tab
- Select **Edit profile** and check/uncheck the **Kiosk mode** box
- **Save** the change

![]({{ site.baseurl }}/assets/smart/image165.png) ![]({{ site.baseurl }}/assets/smart/image168.png)

### Setup for kiosk Mode

1. In SMART Desktop, go to **Field Data \> SMART Mobile \> Install SMART Mobile on Device...**
1. Click the "**\...**" button and browse to the folder where you saved the .APK file and select it and click **Next.**
![]({{ site.baseurl }}/assets/smart/image21.png)
1. Select the option **Configure SMART Mobile as a kiosk.**
1. Click **Next**
![]({{ site.baseurl }}/assets/smart/image22.png)
1. Click **Next.**
1. Now you must install the driver which allows this computer to install kiosk mode onto your device. Select **install / reinstall driver.**
![]({{ site.baseurl }}/assets/smart/image25.png)
1. Right click on "android_winusb" (file type: Setup Information) and select **install.**
![]({{ site.baseurl }}/assets/smart/image24.png)
![]({{ site.baseurl }}/assets/smart/image23.png)
1. Click **Next**

### Provisioning the device

1. **Factory reset the device** by opening settings on your device and selecting "Factory Data Reset".
1. Wait for the device to restart
1. Follow the instructions and press **skip** when asked to create an account.
![]({{ site.baseurl }}/assets/smart/image28.png)
1. Change the time and date back to the correct date and time using the settings on the device.
1. Change the GPS settings in **location** to use GPS only.
![]({{ site.baseurl }}/assets/smart/image26.jpg)
1. Enable "Developer Mode" \> **About phone \> software information** and tap on the build number (or version) 10 times to access **developer mode.**
![A screenshot of a social media post Description automatically generated]({{ site.baseurl }}/assets/smart/image31.png)
1. Enable "USB debugging" by opening the settings, search for USB debugging under developer options and toggle this **on.**
![]({{ site.baseurl }}/assets/smart/image30.jpg)
1. Connect your device to your computer -- select "allow USB debugging" if prompted and select **OK**
1. Configure your device by selecting **"Provision the device"**
1. Click **Finish**
![]({{ site.baseurl }}/assets/smart/image7.png)
1. Launch SMART Mobile

### Exiting Kiosk Mode

Once your mobile device has been configured for kiosk mode, you can only exit out of kiosk mode by:
- Typing in your pin; or
- Factory resetting the device

