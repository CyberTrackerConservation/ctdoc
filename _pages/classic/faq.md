---
layout: page
title: Frequently Asked Questions
nav_order: 50
parent: CyberTracker Classic
permalink: /classic/faq/
---
# Frequently Asked Questions (FAQ)
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### What is CyberTracker?

CyberTracker is a software tool that allows non-programmers to collect
field data with mobile devices. A lesser known capability is that it can
also be used to create digital field guides, because it allows rich
content to be displayed in conjunction with data capture fields. So the
data capture system can also serve as a teaching or reference tool.

### How much does CyberTracker cost?

CyberTracker is freeware. Over the years various organizations have
contributed to the development. Some users commission features for their
own use and these then become available for everyone.

### Where can I get the latest version of CyberTracker?

The most recent version is available on this web
[here](/_pages/classic/download.md). The version numbers are always
incrementing, so 3.200 is more recent than 3.195. If the version is a
test version (not well tested), then it will have "(BETA)" after the
build number.

### CyberTracker contains some GIS functionality, but I need more

CyberTracker is primarily a data capture tool. We've been resisting the
move toward extensive GIS functionality because it distracts from
producing a great data capture solution. We also do not wish to compete
on features with products like ESRI ArcView. If you need more GIS
functionality, we recommend using ArcGIS with CyberTracker as your
data-conduit.

### How do I get new features into CyberTracker?

Email justin@steventon.com with your feature request.

### Which desktop operating system does CyberTracker run on?

CyberTracker runs on all versions of Microsoft Windows, excluding
Windows RT.

### What mobile devices does CyberTracker support?

CyberTracker supports Windows Mobile and Android devices. If you bought
a device in the last 5 years that runs Windows Mobile/CE or Android,
then it will probably work. However, we currently do require touch
screen support, so Smart phones without touch screens are not supported.

### Can I collect data with both Windows Mobile and Android devices at the same time?

Yes. You won't be able to tell which data came from which device (unless
you want to).

### How do I change the screen type, e.g. from radio list to check list?

1.  Click the "Layout" toolbar button
2.  Select the Element List Control
3.  Change the "List mode" property - options are "Single select",
    "Multi select", etc
4.  Click the "Layout" toolbar button again

### How can I install CyberTracker on my Windows Mobile SD card?

When you install the application for this first time, CyberTracker will
install itself onto your device using ActiveSync. At this time, you will
receive message dialog like: "Install CyberTracker Client using the
default application install directory?". Click "No" and you will be
given the option to choose an install location, e.g. Main Memory, SD
Card, etc. If you missed this dialog the first time, just uninstall
CyberTracker from your device (Start-\>Settings-\>System Tab-\>Remove
Programs) and click "Synchronize" again.

### Does CyberTracker support collection of sightings on a laptop or desktop computer?

Yes, you can click on the "New sightings" button in "Report" mode.

### Why can't I edit data in a query table?

Table data is only editable if the column is bound to a single Element
and the Column "Output As" field is set to "Data". If you want to edit
sightings more flexibly, then use the "Edit Sighting" feature off the
Edit menu.

### How do I export sightings that don't have Latitude/Longitude to an ESRI Shapefile?

You can enable dummy XY generation by checking the "Generate XY on
ShapeFile export" feature on the "Advanced" tab of the "Map Settings"
dialog. Select "Edit View" from the toolbar when the map is selected.

### Why don't my sightings save?

Applications require that you have a Save button at the end of them,
i.e. if your Application is: Screen A -\> Screen B -\> Screen C, then
you must have a "Save" button on Screen C. You can enable a save button
by checking the "Show Save 1" or "Show Save 2" checkbox on the screen
properties under the "Navigator" title. Note, typically you will also
uncheck "Show Next" so that your users have no choice but to Save at the
end of a sighting.

### Why do I get the message "Time out of sync"?

It was a common problem that data would have the wrong date/time. Now,
the date/time on your device must be at least as recent as the
Application you want to run. If you get this message often, the most
likely reason is that your device time is wrong. Note, ActiveSync will
automatically synchronize your time if you have a Partnership. Phones
typically pick up the time from the carrier.

### Why do I get the message "Version Error - resync"?

Resource files on the device must be created with the same version of
CyberTracker that is running on the desktop. You should either resync or
delete them.

### When is my data downloaded from my device?

CyberTracker downloads the data during a sync operation. You can force
CyberTracker to download sightings from an attached device using
"File-\>Download Data from Connected Device". If the download completed
without error, then all the sightings are deleted from the device.

### What are timer tracks?

The timer track feature sets up a timer that takes a GPS reading at
fixed intervals. You can customize how long those intervals are from 1
second up. The track system internally has 2 separate modes of
operation: short interval and long interval. For short intervals (60
seconds or less), the device is prevented from going to sleep on it's
own and the GPS is left permanently connected. For long intervals (more
than 60 seconds), the device can be shut down and the alarm system will
be used to wake it up, take a reading and shut it down again.

### How can I edit my timer tracks?

There is no support in the CyberTracker UI for track editing. However,
since the CyberTracker database is a Microsoft Access MDB file, you can
open it and modify the "Waypoint2" table directly.

### How do I make the screen state persist between sightings, e.g. so a list keeps it's selection?

Several controls allow you to persist their state by using their "Retain
state" property. Click the "Layout" toolbar button in "Applications"
mode, select the control and check that property.

### What does the GPS Accuracy number mean?

"Accuracy" is a number that the GPS provides to give some idea of the
uncertainty of the reading. This number ranges from 0 to 50 and should
typically be multiplied by 10 meters (32 feet) to get an idea of the
area you are dealing with. For example, a value of 3.5 means that the
GPS knows you are within 35 meters of where it says you are.

### Does CyberTracker support Differential GPS?

CyberTracker does not have a feature to post-process GPS data. However,
if you are within North America and your GPS is WAAS enabled, then you
get differential like characteristics for free.

### What are the different states for the GPS triangle button?

The GPS triangle has 4 possible states:

1.  Empty triangle with line through it = Track timer is not set and no
    open connection to the GPS exists
2.  Empty triangle with number in it = Track timer is enabled, but last
    track reading was not successful. This could be because the GPS is
    still acquiring satellites, or because the required GPS accuracy was
    not met on last attempt.
3.  Empty triangle with number in it and line through it = track timer
    is set, but the connection to the GPS timed out and so CyberTracker
    is no longer trying.
4.  Filled triangle = Track timer is enabled and last track reading was
    taken successfully

The number in the triangle is the track timer frequency. If the
navigator button size is too small (as is the case on legacy PalmOS),
this may not show. In addition, the display is rounded off, e.g. 80
seconds will show as "1m" (for 1 minute), even although it really is set
at 80 seconds.

### How can I get my RangeFinder and my GPS to both auto-detect without conflict?

If your RangeFinder is Bluetooth, then you cannot also have a Bluetooth
GPS. The way to do this is to turn on your GPS and get it to detect
first. Once CyberTracker has detected the GPS at a particular port, it
will remember that for all future tries. Then do the same for the
RangeFinder.

### What RangeFinders does CyberTracker support?

CyberTracker supports RangeFinders that output the Laser Atlanta NMEA
sentences LA1KA, LA1KC and LA1KD. RangeFinders are not currently
supported on Android.

### How can I export data that I collect back to my GPS?

CyberTracker supports export to CSV (Comma Separated Values) from the
Query Table in Report mode. G7ToWin is a freeware application that can
import CSV files. However, in order for this to work, you need the first
column of your table to be called "Type" and have a "W" for its value.
To make a table have a "W" in the first column, do this:

1.  Find an Element that exists in every sighting, e.g. "Begin"
2.  Go to the "Elements" mode (View-\>Elements)
3.  Find the Element "Begin" and click on "Element Properties" in the
    toolbar
4.  Set the "Tag" property (on the first tab) to "W" (without quotes)
5.  Go to the "Reports" mode (View-\>Reports)
6.  With the Table active, click "Edit View" on the toolbar
7.  Click "Add" to add a new column
8.  Set "Element source" to your Element, set "Name" to "Type" and set
    "Output As" to Tag
9.  Click "Move up" until it is the first column

Now you should have a "W" in the first column of your table. Don't
forget to add "Latitude" and "Longitude" columns as well. Click "Export"
on the toolbar to export.

### What is the difference between a screen and a sub-screen?

Screens and subscreens are identical from the systems point of view.
Grouping is allowed to help the user organize their screens.

### How do Paths work?

A path is created when sightings are connected in the map view. The path
system is configured from the maps "View Properties" dialog under the
"Render" tab. There are 3 Elements which control the path: Start
Element, Stop Element and Join Elements(s).

If you do NOT set the Join Element(s), then the path will be controlled
by the Start and Stop entirely, i.e. a sighting containing the "Start
Element" will begin a path and it will not be terminated until a
corresponding "Stop Element" occurs in a subsequent sighting. If you set
the "Join Elements(s)", then the system will connect any 2 points pA and
pB (with pA occurring before pB) if they meet the following
requirements:

1.  pA and pB must come from the same PDA
2.  pA must not contain the "Stop Element"
3.  pB must not contain the "Start Element"
4.  pA must contain the "Start Element" OR one of the "Join Elements"
5.  pB must contain the "Stop Element" OR one of the "Join Elements"
6.  If pA and pB both contain a "Join Element", then it must be the same
    one

Note, a "Join Element" is defined as an Element that must be in each
sighting for it to be considered part of the same path. The concept is
that we can build different paths out of the same data, depending on
what I want to connect. Some examples:

Connecting observations made by one particular Observer:
```
Set "Join Element(s)" to the Name of the observer
```

Connecting observations by transportation mode, e.g. Walk, Horse, Vehicle:

```
Set the "Join Element(s)" to a category containing the "Walk", "Horse" and "Vehicle" Elements.
Note, this assumes that all your sightings contain the mode of transportation that was used and only one can be used at a time.
```

### How does the Element Formula control work?

The formula property is a regular expression, meaning it can hold
expressions like: "1+2". If you set the formula to this, the output will
be "3". However, there is also support for more complex expressions:

1.  "A+2" (where A is the number value of the Elements in the "Element
    A" property.
2.  "(1 + 2) \* 3" works because parentheses are supported
3.  "max(1, 2)" produces "2" and "min(1, 2)" produces "1"
4.  "abs(-5)" produces 5
5.  "Today" works with the "Output as date" property. "Today-1" is
    yesterday.
6.  "date(2007, 5, 20)" produces a date, see (5).
7.  "if (1 \< 2, 3, 5)" produces "3"
8.  "if (1 \> 2, 3, 5+1)" produces "6"

You can place the result of the calculation in the "Result element",
which will then become part of the sighting data.

If you put the result into a global value using the "Result global
value" property, then you can later reuse that value in the formula
itself. This provides the ability to do counters. Try this:

1.  On screen 1, drop an "Element Formula" control:
2.  Set the "Formula" property to "Test + 1"
3.  Set the "Result global value" property to "Test"

Now everytime you save and return to this screen, the number will
automatically increment.

### How to bind a bluetooth device on Windows Mobile?

On an HP Travel Companion:

1.  Tap Start and then Settings
2.  Tap on the Connections tab
3.  Tap the Bluetooth Icon
4.  Tap "Turn on" to make sure Bluetooth is enabled
5.  Tap on the "Bluetooth Manager" shortcut near the bottom of the
    screen
6.  Turn on the device you want to bind to and tap "New" on the bottom
    left corner of the screen
7.  Tap "Explore a Bluetooth device" and tap "Next" 8. An icon should
    appear that describes the device you want to bind to. There may be
    multiple devices, but just select the one you want and tap "Next".
    Sometimes the screen will automatically press the next button for
    you.
8.  Uncheck "Use a secure, encrypted connection"
9.  Under "Service selection", select "Bluetooth Serial Port" and tap
    "Next".
10. You may be asked to enter a password. The device documentation
    provides this. Usually it is "0000" or "1111".

On a Trimble GeoXM:

1.  Tap Start and then Settings
2.  Tap on the Connections tab
3.  Tap the Bluetooth Icon
4.  Select "On"
5.  Select the "Bonded Devices" tab
6.  Select the "New" list item
7.  Select the device you want to bind to and tap "Next"
8.  Enter the passcode for the device. This can be found in the device
    manual. Usually it is "0000" or "1111".
9.  Tap "Next" to create the shortcut
10. Close the input field and tap on the "Serial Ports" tab
11. In the "Client Serial Ports" box, tap "New"
12. Select the device and tap "Next"
13. Make sure "Authentication", "Encryption" and "Default Bluetooth
    ActiveSync" are all unchecked
14. Click "Finish"

### What does "No Result: Value not saved" and "No Result: Text not saved" mean?

Text and Keypad screens require that the "Result Element" property be
set. This specifies the storage Element for the result from the text
editor and keypad screens. The error message occurs to prevent
accidental data loss.

### What is "Kiosk Mode" and how can I set it up?

Kiosk's are fixed purpose devices. The goal of Kiosk mode is to turn a
device into a fixed purpose CyberTracker device. To configure this, open
the "Application Properties" dialog during screen design and check the
"Kiosk Mode" box. Save your database and synchronize the Application to
your device. Notice that the application cannot be closed in the usual
ways. The task bar is also hidden.

Kiosk mode is often combined with a password keypad to allow
administrators to work on the system in the field.

### How can "Kiosk Mode" be bypassed in the field?

Place an "Element Keypad" control on a screen and set the "Password"
property to "1234". Set the "Password auto next" property to "Shutdown".
When the correct password is entered, CyberTracker will close the
current Application, thereby terminating Kiosk mode.

### CyberTracker reports that it cannot install to a Windows Mobile device: INF error

To install CyberTracker on the device manually:

1.  On the desktop CyberTracker icon, right click and select "Open File
    Location"
2.  Look for client5.arm.cab and copy this file to your Windows Mobile
    6.1 device
3.  Open File Explorer on the device and navigate to the file, then
    double tap it

This should install CyberTracker. After this, the desktop should
communicate with it properly.
