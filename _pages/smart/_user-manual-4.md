## Prerequisites

To use SMART Mobile:

- You must have installed SMART Desktop version 7.5 or higher (earlier versions are not supported).
- Android version 6.0 or higher: you can view what Android version you have in the device's System Settings.
- iOS version 14.x for SMART Connect only. This makes use of wireless connectivity, uploading configurable models via the SMART Connect server. For iOS on your device go to Settings \> General \> About.
- If you use SMART Connect, you will need SMART Connect version 6.3 or higher (earlier versions are not supported). 
- You must decide whether you want to use the kiosk mode version or the non-kiosk mode version of SMART Mobile (see below).

{: .important }
SMART Mobile is available in a kiosk mode version for Android devices. This version needs to be specifically chosen and requires additional steps to set up so it is imperative that you decide whether or not this is necessary before selecting the version of SMART Mobile you plan to use (e.g. kiosk vs. non-kiosk).


## SMART Mobile setup 

{: .note }
If you decide to use kiosk-mode please navigate to setup instructions for kiosk mode. The following instructions are for the non-kiosk version of SMART Mobile.

### Prepare to install SMART Mobile

Before you install SMART Mobile on an android device you need to prepare your android handheld device. On your Android handheld device, you need to:

1. Have a file manager: Any file application, pre-installed or downloaded, that allow one to browse folders on the device should work.
1. Enable "Use Unknown Sources"
- From a Home screen, swipe up or down from the center of the display to access the apps screen.
1. Navigate: Settings \> Apps
1. Tap Menu icon (upper-right)
1. Tap Special access
1. Tap **Install unknown** apps
1. Select the **unknown** app then tap the **Allow** from this **source** switch to **turn on**
- Set the location mode to device only
1. In the device Settings go to Security & Location
- May differ between Android versions
1. Under Privacy go to Location.
1. Set Location Mode to Device only (use GPS to determine location).

**If you ARE using SMART Connect, proceed to 4.2.2. If you ARE NOT using SMART Connect at your site, proceed to 4.2.3.**

### Prepare your SMART Connect for SMART Mobile

1. Sync all your desktop and Connect SMART instances and all local data on your desktop is synced with your Connect instance.
1. Backup your existing SMART desktop database.
1. Backup your existing SMART desktop database using the **File \> Backup System** menu option.

{: .warning }
To avoid losing data, before making any changes to SMART, always sync your desktop and make a backup of your Conservation Area.

### Setup in non-kiosk mode

You will set up your device with SMART mobile then learn the procedures for using the app to collect observational data.

A. Uninstall any previous version of SMART Mobile (if applicable).

B. Download the latest SMART Mobile application file from the SMART website -- www.smartconservationtools.org.

{: .hint }
We are continuously working to make SMART Mobile better. Newer builds may be released with bug fixes and UX improvements. **We recommend that you use the latest build when possible.**

C. Save the .APK file in an easily found location on your computer (e.g., the same root folder as your SMART Desktop installation). Connect your mobile device to your computer. In SMART Desktop, go to **Field Data \> SMART Mobile \> Install SMART Mobile on Device...**

**NOTE: This wizard will overwrite the existing APK on your device with the most current version. (Fig. 11)**

  > ![]({{ site.baseurl }}/assets/smart/image105.png){: width="40%" }

D. Click the "**\...**" button and browse to the folder where you saved the APK file and select it and click **Next.**

  > ![]({{ site.baseurl }}/assets/smart/image21.png){: width="40%" }

E. Select the option **Copy SMART Mobile to Device**.

F. Click **Next**

  > ![]({{ site.baseurl }}/assets/smart/image159.png){: width="40%" }

G. Select the device you would like to export to. If the device is not shown check that it is in file transfer mode and refresh the list. Always select **internal storage** if given the option of SD card. Ensure to de-select SD card option.

  > ![]({{ site.baseurl }}/assets/smart/image83.png){: width="40%" }

H. Click **Copy application to selected devices. This ends the desktop setup, now go and** check your device for the SMART Mobile application.

  > ![]({{ site.baseurl }}/assets/smart/image154.png){: width="40%" }

I. Now looking at your device, install the SMART Mobile Application (see screenshot examples below)
1. On your Android device, use the file manager to find the SMART Mobile APK file.
1. Select the SMART Mobile APK file to launch the installation.
1. Select **Install**
1. Once the installation has finished, select **Done**. 
1. You will be prompted to "delete the installation package". Click **Yes**.

  > ![]({{ site.baseurl }}/assets/smart/image176.png){: width="80%" } 
  > ![]({{ site.baseurl }}/assets/smart/image179.png){: width="80%" }

J.  You may be prompted to switch your Android device's home launcher app to SMART. **If you receive this message, do [NOT] select switch launcher apps.** (Note: This prompt may be different on your device.)

  > ![]({{ site.baseurl }}/assets/smart/image178.png){: width="40%" }

K. Launch SMART Mobile

  > ![]({{ site.baseurl }}/assets/smart/image20.png){: width="80%" }

### SMART Mobile setup after installation to the device

**Choose a configurable model for data collection**

Depending on the mandate for the patrol, you will select a data model
for use with collecting data. The data model will include relevant
categories and attributes of data that are to be collected. Designing
data models is a topic for advanced administration. Here we will simply
take a look at the configurable model and see what it contains.

**Reminder:** The **Data Model** for a Conservation Area is made up of
all the possible categories and attributes you may want to record when
making an observation. A **Configurable Model** is how the **Data
Model** can be edited to appear for different patrol mandates, i.e. law
enforcement, research or wildlife monitoring. For more information, see:
*[[SMART 6 Technical Training
Manua](https://smartconservationtools.org/wp-content/uploads/2019/07/SMART%206%20Technical%20Training%20Manual_2019_07_sm.pdf)l,]*
*Module 9: Data Model Management*

1. From SMART Desktop Select **Conservation Area \> Configurable model \> *'Name of model'***.
1. Click edit to inspect the categories and attributes associated with the model
1. Check to make sure the SMART Mobile settings follow what you see below by selecting **'Field Data-\>CyberTracker Classic-\>CyberTracker Properties'** in SMART. 
1. Kiosk Mode on or off as per choice made in Section 4.1 above
1. Track Timer can be between 3 and 10 secs
1. Set GMT/UTC time offset for your location
1. If you make any edits to the settings, make sure to select **Save**

{: .note }
For SMART 7 these configurations apply to both SMART Mobile and Cybertracker Classic. You will configure properties for both here.

  > ![]({{ site.baseurl }}/assets/smart/image8.png){: width="80%" } 
  > ![]({{ site.baseurl }}/assets/smart/image5.png){: width="80%" }

### Additional Configurable Model Features

#### Language

SMART Mobile, unlike Classic CyberTracker, is capable of rendering any Unicode language as text on the device. In order to do this, you need to edit the text of your configurable model. Open a configurable model, select **Edit** and select all the categories and attributes, one-by-one, and simply type in whatever language you want displayed on the device. 

![]({{ site.baseurl }}/assets/smart/image3.png){: width="40%" }

#### Icons

Creating and exporting configurable models to SMART Mobile is much the
same as for CyberTracker Classic. However, SMART Mobile enables the use
of icons which display on the device instead of, or alongside, text in
order to assist in cases where field staff are unable to read the
instructions or work better with images. In order to enable these on
your device you need to edit your configurable model. 

In SMART Mobile version 3xx there are an additional yy icons available
to choose from.

Locate the configurable model you plan to export to your device and
select **Edit.** For each group, category and attribute you are able to
decide whether you want to display text, image or both text and image.
SMART comes pre-loaded with a set of icons for the default data model.
If your data model uses the same category you can simply use "**Image:
Data Model (Default Image)**". If your data model does not have a
default image (or you would prefer a different icon) you can do this by
selecting "**Custom**" under "**Image**". You can then select an icon
from your hard drive (or select another built-in SMART icon) and
associate this with your group, category or attribute. 

![]({{ site.baseurl }}/assets/smart/image6.png){: width="40%" }
![]({{ site.baseurl }}/assets/smart/image2.png){: width="40%" }
![]({{ site.baseurl }}/assets/smart/image13.png){: width="40%" }

Once you're happy with the structure and design of your configurable
model click **Save**.
