# Installation and Use

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

C. Save the .APK file in an easily found location on your computer (e.g., the same root folder as your SMART Desktop installation). Connect your mobile device to your computer. In SMART Desktop, go to **Field Data \> SMART Mobile \> Install SMART Mobile on Device...**

{: .hint }
SMART Mobile is continually improving. Newer builds may be released with bug fixes and other improvements. **When possible, use the latest build.**

{: .note }
This wizard will overwrite the existing APK on your device with the most current version. (Fig. 11)

  > ![]({{ site.baseurl }}/assets/smart/image105.png){: width="75%" }

D. Click the "**\...**" button and browse to the folder where you saved the APK file and select it and click **Next.**

  > ![]({{ site.baseurl }}/assets/smart/image21.png){: width="75%" }

E. Select the option **Copy SMART Mobile to Device**.

F. Click **Next**

  > ![]({{ site.baseurl }}/assets/smart/image159.png){: width="75%" }

G. Select the device you would like to export to. If the device is not shown check that it is in file transfer mode and refresh the list. Always select **internal storage** if given the option of SD card. Ensure to de-select SD card option.

  > ![]({{ site.baseurl }}/assets/smart/image83.png){: width="75%" }

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

**Language**

SMART Mobile, unlike Classic CyberTracker, is capable of rendering any Unicode language as text on the device. In order to do this, you need to edit the text of your configurable model. Open a configurable model, select **Edit** and select all the categories and attributes, one-by-one, and simply type in whatever language you want displayed on the device. 

  > ![]({{ site.baseurl }}/assets/smart/image3.png){: width="75%" }

**Icons**

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

  > ![]({{ site.baseurl }}/assets/smart/image6.png){: width="40%" }
  > ![]({{ site.baseurl }}/assets/smart/image2.png){: width="40%" }
  > ![]({{ site.baseurl }}/assets/smart/image13.png){: width="40%" }

Once you're happy with the structure and design of your configurable
model click **Save**.

## Kiosk mode

Kiosk mode is a function which locks your device to the function of a specific application and prevents the use of any other application. Essentially, using kiosk mode will turn your device into a SMART-Mobile-Only device.

**When to use kiosk mode**

Deciding whether to use kiosk mode is highly dependent on your
particular use case. If you feel it is necessary to lock a device to
SMART Mobile only then kiosk mode is for you. This might be to ensure
that devices procured for SMART data collection are used only for this
function and nothing else. By dedicating your mobile device for SMART
mobile data collection, kiosk mode simplifies data collection, focuses
attention on that task alone, and conserves device resources.

**When not to use kiosk mode**

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

  > ![]({{ site.baseurl }}/assets/smart/image199.png){: width="75%"}

- Select **Edit** and go to the **CyberTracker** properties tab

- Select **Edit profile** and check/uncheck the **Kiosk mode** box

- **Save** the change

  > ![]({{ site.baseurl }}/assets/smart/image165.png){: width="40%"} ![]({{ site.baseurl }}/assets/smart/image168.png){: width="40%"}

### Setup for kiosk Mode

1. In SMART Desktop, go to **Field Data \> SMART Mobile \> Install SMART Mobile on Device...**

2. Click the "**\...**" button and browse to the folder where you saved the .APK file and select it and click **Next.**
  > ![]({{ site.baseurl }}/assets/smart/image21.png){: width="75%"}

3. Select the option **Configure SMART Mobile as a kiosk.**

4. Click **Next**
  > ![]({{ site.baseurl }}/assets/smart/image22.png){: width="75%"}

5. Click **Next**

6. Now you must install the driver which allows this computer to install kiosk mode onto your device. Select **install / reinstall driver**.
  > ![]({{ site.baseurl }}/assets/smart/image25.png){: width="75%"}

7. Right click on "android_winusb" (file type: Setup Information) and select **install.**
  > ![]({{ site.baseurl }}/assets/smart/image24.png){: width="75%"}
  > ![]({{ site.baseurl }}/assets/smart/image23.png){: width="40%"}

8. Click **Next**

### Provisioning the device

1. **Factory reset the device** by opening settings on your device and selecting "Factory Data Reset".
2. Wait for the device to restart
3. Follow the instructions and press **skip** when asked to create an account.
  > ![]({{ site.baseurl }}/assets/smart/image28.png){: width="75%"}
4. Change the time and date back to the correct date and time using the settings on the device.
5. Change the GPS settings in **location** to use GPS only.
  > ![]({{ site.baseurl }}/assets/smart/image26.jpg){: width="40%"}
6. Enable "Developer Mode" \> **About phone \> software information** and tap on the build number (or version) 10 times to access **developer mode.**
  > ![]({{ site.baseurl }}/assets/smart/image31.png){: width="75%"}
7. Enable "USB debugging" by opening the settings, search for USB debugging under developer options and toggle this **on.**
  > ![]({{ site.baseurl }}/assets/smart/image30.jpg){: width="40%"}
8. Connect your device to your computer -- select "allow USB debugging" if prompted and select **OK**
9. Configure your device by selecting **"Provision the device"**
10. Click **Finish**
  > ![]({{ site.baseurl }}/assets/smart/image7.png){: width="75%"}
11. Launch SMART Mobile

### Exiting Kiosk Mode

Once your mobile device has been configured for kiosk mode, you can only exit out of kiosk mode by:
- Typing in your pin; or
- Factory resetting the device

## Overlay of Internet Map Layers

WMS layers can be configured in the "Basemap Settings" under the package. There are many public layers available, for example:

-   https://nowcoast.noaa.gov/arcgis/services/nowcoast/radar_meteo_imagery_nexrad_time/MapServer/WMSServer

  > ![]({{ site.baseurl }}/assets/smart/image14.png){: width="40%"}

## Track timer settings

The desktop can configure different track timer settings for each patrol
type. The value of this setting can be seen on the map screen:

  > ![]({{ site.baseurl }}/assets/smart/image18.png){: width="40%"}

## Creating a Package

Now that you have created your configurable model that can be used to efficiently collect your data, you can export your Data Collection Package from your SMART desktop to your mobile device as follows:

[There are two options, manual export via a USB connection, or download
direct from SMART connect]

**Manual export via USB connection**

1. Open your SMART database.
2. Connect your mobile device to your computer USB port using the device's download cable
3. Make sure the device is connected for 'file transfer'
4. Export the configurable model you will be using by clicking, "Field Data-\>SMART Mobile-\>Packages"... and then on the SMART Mobile Packages dialog that allows you to export either Local or Connect packages click on +Add and select Patrol Package as your SMART Mobile Package Type.
  > ![]({{ site.baseurl }}/assets/smart/image131.png){: width="75%"}
  > ![]({{ site.baseurl }}/assets/smart/image153.png){: width="40%"} ![]({{ site.baseurl }}/assets/smart/image49.png){: width="40%"}

5. Set "Export Location" as "Device".
6. Choose your Configurable model and CyberTracker Properties.
7. Select your preferred basemap (Leave min/max at the defaults, and lower the "Max" to number (e.g., to 1 or 2) to speed up the export).
8. Check Collect Independent Incidents and select your Configurable Model an Independent Incident Model if you wish to enable this option.
9. Click "Export..."
  > ![]({{ site.baseurl }}/assets/smart/image60.png){: width="75%" }
  > ![]({{ site.baseurl }}/assets/smart/image62.png){: width="75%" }
  > ![]({{ site.baseurl }}/assets/smart/image61.png){: width="75%" }

10. Disconnect the device.
11. Open SMART Mobile on your device. 
12. Click **SMART Mobile** on the **Connect** screen. This will scan your device for new projects. Your configurable model should autoload in the **Projects** screen and be ready for use.

  > ![]({{ site.baseurl }}/assets/smart/image63.png)

{: .note }
When updating a configurable model (for example to add new employees added to list) and needing to update the devices, if it is the same patrol package name, SMART Mobile will overwrite it. Just go through the same workflow as before to export the configurable model to the device.

## SMART Mobile Desktop Simulator Instructions for Windows (64 Bit)

The SMART Mobile simulator runs on Windows desktop and is intended to help with training and testing. To get started, follow the following steps:

1. Download the zipped SMART Mobile simulator program files
2. The SMART Mobile desktop simulator is available at [www.smartconservationtools.org](http://www.smartconservationtools.org)
3. Extract the files to a local folder on your computer.
4. Open SMART desktop and export a Patrol Package to file:
- When exporting to a file, set the file location to \"C:\\users\\\<YourName\>\\Downloads\" or \"C:\\users\\\<YourName\>\\Desktop\", being sure to replace <YourName\> with whatever your local user name on the machine is.
- The file name is not important, as long as it ends in .zip. When the desktop simulator processes the file, it will remove it from the directory.
- The exported file MUST have a ZIP extension
  > ![]({{ site.baseurl }}/assets/smart/image16.png){: width="75%"}
  > ![]({{ site.baseurl }}/assets/smart/image51.png){: width="75%"}

5. Navigate to the location where you extracted the SMART Mobile simulator program files and open the executable file (SMART_Mobile.exe).
  > ![]({{ site.baseurl }}/assets/smart/image57.png){: width="75%"}

6. The simulator will open as it would display on a mobile device.
  > ![]({{ site.baseurl }}/assets/smart/image58.png){: width="40%"} 

7. Click on the configurable model and run SMART Mobile on the desktop.

## Preparing to record observations

1. Turn on the SMART Mobile-equipped device
2. Turn on the GPS on the device.
3. Start the SMART Mobile application by tapping on the SMART Mobile icon on your home screen:
  > ![]({{ site.baseurl }}/assets/smart/image64.png)

4. Tap on the configurable model for the field activity you want to undertake.

{: .note }
SMART Mobile can accommodate multiple configurable models for example for different patrol mandates or objectives. In the example below the device can be used either for recording law enforcement or wildlife patrols, each with its own unique configuration.

If you need to exit from SMART Mobile after you have selected the configurable model enter the default exit pin code **"1234**" and press the green button, or have your SMART data manager enter the correct pin code. See [SMART Technical Training
Manual](https://smartconservationtools.org/wp-content/uploads/2019/07/SMART%206%20Technical%20Training%20Manual_2019_07_sm.pdf): Module 9: CyberTracker Plug-In and Smart Mobile* for more details on pin codes and 'Kiosk mode'.

> ![]({{ site.baseurl }}/assets/smart/image52.png){: width="40%" } ![]({{ site.baseurl }}/assets/smart/image35.png){: width="40%" }

After selecting the configurable model, you are ready to begin recording the Patrol Configuration

1. Select **Start Patrol** then you will see a screen to enter the patrol configuration
2. The GPS automatically starts to look for satellites and will return the location after achieving a 3D fix
- SMART Mobile will not allow a patrol to start until it has gotten a location (i.e., you will see coordinate in the "Location" box). This may take a few minutes if the device is new and getting a GPS location for the first time or hasn't been used recently.
  > ![]({{ site.baseurl }}/assets/smart/image37.png){: width="40%" } ![]({{ site.baseurl }}/assets/smart/image36.png){: width="40%" }

3. Use the dropdown menus to select the associated metadata:
    -   patrol transport type
    -   armed status
    -   team name
    -   station name
    -   patrol mandate

4. First select values for patrol transport type
5. Then select the team name
6. Then select the station name
  > ![]({{ site.baseurl }}/assets/smart/image38.png){: width="30%" } ![]({{ site.baseurl }}/assets/smart/image48.png){: width="30%" } ![]({{ site.baseurl }}/assets/smart/image41.png){: width="30%" }

7. Then select the **Patrol Mandate**. This will correspond with the configured data model being used

8. For **Employees** scroll down the list and check the boxes next to the names of staff participating in the patrol

9. Select the **Leader** by highlighting his/her name, then click the arrow in the upper left of the screen to go back to the Employees menu, then check the tick box in the upper right of the screen:
  > ![]({{ site.baseurl }}/assets/smart/image39.png){: width="30%"} ![]({{ site.baseurl }}/assets/smart/image42.png){: width="30%"} ![]({{ site.baseurl }}/assets/smart/image46.png){: width="30%"}

10. If you want to specify objectives or comments those will require entering text into the relevant fields, then check the tick box in the top right of the screen:
  > ![]({{ site.baseurl }}/assets/smart/image34.png){: width="40%"} ![]({{ site.baseurl }}/assets/smart/image32.png){: width="40%"}

11.  When you are finished entering the patrol configuration check the tick box in the top right of the screen. This will take you to the Patrol screen from where you can begin to record observations:
  > ![]({{ site.baseurl }}/assets/smart/image81.png){: width="40%" }

## Recording observations using SMART Mobile

From the patrol screen you may end, pause or change your patrol, simply select "Patrol" to enter the menu at the bottom of your screen.

You should select **Pause patrol** when the team is not actively engaged in search activity for example when taking a meal break, when waiting for radio orders from a patrol supervisor, or if a vehicle is broken down. You can only pause a patrol if you checked the pause patrol box in the Cybertracker settings. Hit **Pause patrol** again to restart the
patrol after it was paused.

{: .note }
The 'Pause Patrol' function must be enabled in the CyberTracker properties for it to be visible on patrol (See Section 4.2.5 -- above).

  > ![]({{ site.baseurl }}/assets/smart/image90.png){: width="40%" } ![]({{ site.baseurl }}/assets/smart/image86.png){: width="40%" }

You may want to change the transport type, mandate, employees or leader during the patrol as the situation requires. A significant enhancement in SMART Mobile is the ability to change patrol metadata during the patrol. For example, if your patrol began as a foot patrol and later continued by vehicle, you would use this function to change your patrol transport type from "foot" to "vehicle" with the ease of a few taps, rather than having to end and restart your patrol with different data. The device will make a note of when and where this occurred for more accurate information on your patrols. Once you download the data to SMART, the different sections of the patrol will automatically display
as different patrol legs.

You would select **End patrol** after you have completed your patrol route, have returned to your station or have stopped recording observations and do not plan to resume again for the rest of the day or evening.

  > ![]({{ site.baseurl }}/assets/smart/image87.png){: width="40%" }

During a patrol you can also access the following functions: 

1.  **Map**: Check your GPS location while on patrol and view bservation locations and the tracklog

2.  **History**: Check the observations that were recorded during the patrol

3.  See individual observations, times & dates

  > ![]({{ site.baseurl }}/assets/smart/image93.png){: width="30%" } ![]({{ site.baseurl }}/assets/smart/image89.png){: width="30%" } ![]({{ site.baseurl }}/assets/smart/image94.png){: width="30%" }

## Detailed Steps for Recording Observations using SMART Mobile

Select 'Make observation' at the top of the screen to record patrol observations (below a) relating to SMART data model categories (wildlife, human activities, features and patrol movements etc). In the example below an observation of human activity is recorded b) then details of people encountered is recorded c) along with a photo d).

To finish entering data for an observation select the tick box at the top right of the screen (see red box in top-right of d below). Once the observation has been recorded, save the incident selecting the green button at the bottom right of the screen (below e).

a) ![]({{ site.baseurl }}/assets/smart/image95.png){: width="30%" }
b) ![]({{ site.baseurl }}/assets/smart/image88.png){: width="30%" }
c) ![]({{ site.baseurl }}/assets/smart/image80.png){: width="30%" }
d) ![]({{ site.baseurl }}/assets/smart/image82.png){: width="30%" }
e) ![]({{ site.baseurl }}/assets/smart/image69.png){: width="30%" }

**Multiple observations** can be made at each location (incident). Each time a new observation is added select 'Make Observation'.

In the example below, a **[person]** was encountered at a **[camp]** with a **[wildlife carcass]**. This
represents three unique pieces of data (observations) at one location/event (incident) that should be collected as part of the data model. To begin, the observer first enters the relevant details for the person (below a-d) and clicks on the white check in the top right of the screen (below d). This completes the data entry for Observation #1 (the person) at the incident. The observer would then go through the process again for both the camp (e-h) and the carcass (i-l), making sure that each time the relevant details of the observation are recorded. After entering all of the relevant data for each observation and ticking the white check at the top of the screen, the observation will appear in list of observations recorded at that incident (below m). Note, that below in (m), both 'Camp' and "Carcass" appear beneath
"People -- direct observation". Once all observations have been recorded at the incident, save the incident selecting the green button at the bottom right of the screen (below m).

a) ![]({{ site.baseurl }}/assets/smart/image71.png){: width="30%" }
b) ![]({{ site.baseurl }}/assets/smart/image70.png){: width="30%" }
c) ![]({{ site.baseurl }}/assets/smart/image74.png){: width="30%" }
d) ![]({{ site.baseurl }}/assets/smart/image73.png){: width="30%" }
e) ![]({{ site.baseurl }}/assets/smart/image77.png){: width="30%" }
f) ![]({{ site.baseurl }}/assets/smart/image79.png){: width="30%" }
g) ![]({{ site.baseurl }}/assets/smart/image65.png){: width="30%" }
h) ![]({{ site.baseurl }}/assets/smart/image68.png){: width="30%" }
i) ![]({{ site.baseurl }}/assets/smart/image92.png){: width="30%" }
j) ![]({{ site.baseurl }}/assets/smart/image66.png){: width="30%" }
k) ![]({{ site.baseurl }}/assets/smart/image119.png){: width="30%" }
l) ![]({{ site.baseurl }}/assets/smart/image127.png){: width="30%" }
m) ![]({{ site.baseurl }}/assets/smart/image125.png){: width="30%" }

## Groups

Groups allow input of grouped observations at a single point. This is
available when:

-   "Incident Group UI" is enabled in the Device Settings

  > ![]({{ site.baseurl }}/assets/smart/image123.png){: width="40%" }

\<\<ADD IN SCREENSHOT FROM SMART \>\>

## Signatures

Signature fields must be configured on SMART desktop. This is what it
looks like on Mobile:

  > ![]({{ site.baseurl }}/assets/smart/image126.png){: width="40%" } ![]({{ site.baseurl }}/assets/smart/image124.png){: width="40%" }

## Audio capture

If attachments are allowed for a category, then you will be able to add one or more pictures and an audio note:

  > ![]({{ site.baseurl }}/assets/smart/image141.png){: width="40%" }

## Maps

SMART mobile allows you to use your device for navigation with a multi-featured map;

- Sightings, Incidents, Tracks are visible
- Offline maps overlaid on base map
- 10 online base maps: OpenStreetMap, National Geographic, Satellite, Oceans, etc.
- Offline mode where no basemap is required
- Layers can be turned on and off
- Inspect
- Navigation with realtime pointer
- Compass
- Detailed data
- Satellite view
- Smooth panning, pinch-zoom and rotation
- Rotate to north at top button 
- Zoom in, zoom out buttons
- Follow modes: user, follow, navigation
- Co-ordinates in decimal degrees, degrees minutes seconds, degrees decimal minutes and UTM
- Manual GPS by dropping a point on the map
- Distance and direction

### Manual GPS by dropping a point on the map

The location can be set manually by long pressing on the map. This is available when:

- "Use instantaneous GPS points" is enabled in the Configurable Model settings
  > ![]({{ site.baseurl }}/assets/smart/image139.png){: width="50%" }

- "Manual GPS on skip via input" is enabled in the Device Settings. This means you do not need to be standing in the same location as the point you want to record:

  > ![]({{ site.baseurl }}/assets/smart/image143.png){: width="40%" } ![]({{ site.baseurl }}/assets/smart/image138.png){: width="40%" }

### Distance and Direction

Sighting distance and direction can be set when:

- "Record Distance (m) and Bearing (degrees)" is enabled in the Data Collection Options dialog

  > ![]({{ site.baseurl }}/assets/smart/image134.png){: width="40%" }

### Offline maps
By default, the “SMART Basemap” feature generates an offline map based on the map in SMART. If this is not sufficient, custom offline maps can be added to the SMART Mobile Package.
SMART Mobile supports MapBox (.mbtiles) and ArcGIS (.tpk, .vtpk) offline maps.
To enable them, on the Package dialog, select the “Basemap Settings” tab, then add layers from your machine.

![Image]({{ site.baseurl }}/assets/smart/offline-maps-1.png)

During the next package upload, these files will be available via the Layers menu (bottom left):

|:-------------|:-------------|
| ![Image]({{ site.baseurl }}/assets/smart/offline-maps-2.png) | ![Image]({{ site.baseurl }}/assets/smart/offline-maps-3.png) |

{: .note }
Note that it can be helpful to disable the online layers by selecting “None”. This will enable only the offline layers.

## Independent Incidents

SMART Mobile allows you to collect data not associated with a patrol, on a handheld device. To use this feature, you will need to install the 'Independent Incident' plugin to your SMART database via the '**File \Install New Plugins**' menu. Once you have done this, you can re-export your patrol package and select a configurable model to be used for independent incidents which can differ from your chosen patrol model. For more information on independent incidents see: *[[SMART 6
Technical Training
Manua](https://smartconservationtools.org/wp-content/uploads/2019/07/SMART%206%20Technical%20Training%20Manual_2019_07_sm.pdf)l] Module 11: Independent Incident Plug-in.*

## Mobile data export from device

To export data collected from SMART Mobile to your computer:

1. Click "Export Data" in SMART Mobile
  > ![]({{ site.baseurl }}/assets/smart/image136.png){: width="75%" }

2.  SMART Mobile will create one or more JSON files for each project and place it in a new folder called "/SMARTdata"
  > ![]({{ site.baseurl }}/assets/smart/image137.png){: width="75%" }

## Importing SMART Mobile patrols into SMART 

It is not necessary to use SMART mobile in a connected environment. SMART mobile data collection can be done outside of telephone 3G or 4G networks. However, if you are using SMART Connect with the data queue wifi settings enabled (see the Advanced Administration with SMART connect training handbook) simply ending your patrol will send data to
the data queue which can be downloaded directly into SMART desktop.

For offline use, to import the data collected in SMART Mobile directly to SMART Desktop:

1. Connect your mobile device to your computer using the cable
2. Make sure device is connected for 'file transfer'
3. Open SMART Desktop and go to **Field Data\>SMART Mobile\>Import...**
  > ![]({{ site.baseurl }}/assets/smart/image135.png){: width="75%" }

4. Select to **Import From** your **Device** and SMART will automatically pull your data from your device.
  > ![]({{ site.baseurl }}/assets/smart/image132.png){: width="75%" }

5. Alternatively you can transfer the data from the SMARTDATA folder on the device to a folder on the desktop, and from there Import from Files to SMART. Click the Green cross and select the file to import.
  > ![]({{ site.baseurl }}/assets/smart/image133.png){: width="75%" }

6. Once the file is ready for import select whether you want to Create a New Patrol or Add to Existing Patrol Leg
  > ![]({{ site.baseurl }}/assets/smart/image106.png){: width="75%" }

7. Once imported the New Patrol will appear in the list of patrols in the Patrol View
  > ![]({{ site.baseurl }}/assets/smart/image103.png){: width="75%" }

## Report bugs and other feedback on SMART Mobile 

The SMART Mobile app you are using is a public release version. It has already received extensive field use and testing, however, there remains the possibility of glitches. Please report all bugs and any general comments (e.g., "Feels like too many clicks to get from X to Y") about your experience using SMART Mobile following the steps below. This will ensure we efficiently address all comments/concerns to improve SMART Mobile.

Compile the relevant details about the bug reported or your user experience feedback in an email:

1. In the **Subject** of the email:
- Enter a short description of the bug or feedback.

2. In the **Body** of the email, provide a more detailed description of the bug reported including the following information:
- SMART Mobile version and build installed (e.g., Build 261)
- Mobile device used
- For bugs
- What behavior was expected
- Steps to reproduce the issue
- Feedback on if the issue is a blocker to further use
    - Your name (so we can contact you with any questions about your bug report or feedback)
- Add any relevant **Attachments** to the email, such as:
    1.  Screenshots
    2.  Bug report zip file exported from SMART Mobile

3. Send your email to [smartpm@smartconservationsoftware.org](mailto:smartpm@smartconservationsoftware.org)
 
You may be contacted with follow up questions or requests to retest to confirm the bug you reported has been successfully resolved.

**Creating a bug report in SMART Mobile**

1. In SMART Mobile, go to **Settings** and click **Report a Bug**
2. Write a brief description of the bug and click the **Save check mark**
3. SMART Mobile will create a zip file with the bug report (including details about your SMART Mobile configuration) and place it in a new folder called "/SMARTdata"
  > ![]({{ site.baseurl }}/assets/smart/image111.png){: width="90%" }

If you need assistance with using SMART mobile, please contact the SMART Program Manager
([smartpm@smartconservationsoftware.org](mailto:smartpm@smartconservationsoftware.org)).

## Exporting patrol data for sharing

After importing the SMART Mobile patrol data to SMART you will export
the patrol to a separate folder in your computer which you may need to
do to share data between computers:

1. Create a folder in your computer with the name of your team-SMART Mobile equipped device or phone number-date of patrol. Example: RukwaLuafi1-BVG2-21April2020. 

2. Open the SMART software \click on **Patrol** on menu bar \click on **Export Patrols** \select the **patrol** or **multiple patrols** you want to export from the drop-down list by clicking on them (a tick mark will appear in front of the selected patrol) \click on **Browse** \Select the folder you created (Example: RukwaLuafi1-BVG2-21April2020) \Click on **OK** \\click on **Export**.

3. The patrol data may be shared via USB or email with data manager for importing into another SMART database.
  > ![]({{ site.baseurl }}/assets/smart/image115.png){: width="75%" } 
  > ![]({{ site.baseurl }}/assets/smart/image104.png){: width="75%" } 
  > ![]({{ site.baseurl }}/assets/smart/image102.png){: width="75%" }

## Field exercise: Data collection using SMART Mobile equipped devices

- Divide into teams to conduct a practice patrol around the training site
- Collect data on the handheld devices; record the patrol configuration, then start taking observations at simulated crime scenes
- Try to be vigilant and observant, especially for signs of human activity, wildlife, and features. Also record the start and end of a patrol, and any changes in movements of the patrol teams such as rest stops or change of transportation (foot to vehicle, vehicle to foot etc.)
- When the patrol is finished, import your data to SMART via the SMART Mobile or CyberTracker field data interface. Compare patrol results between teams. 