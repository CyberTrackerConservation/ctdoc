---
layout: page
title: Change History
nav_order: 80
parent: CyberTracker Classic
permalink: /classic/change-history/
---
# Change History

### 3.522: 05/19/2022

New features:

  - Element Lists in check box mode can output a semi-colon delimeted list of selected items into their "Radio element" property. 

Bug fixes

  - Element names on Filters should update

### 3.521: 02/21/2022

Bug fixes

  - ESRI Connector requries https
  - Too many track points result in out of memory errors

### 3.520: 11/19/2021

Bug fixes

  - Support for Android 11

### 3.518: 10/14/2021

Bug fixes

  - Repoint wiki links
  - Remove telemetry which showed scripting errors

### 3.517: 08/27/2021

Bug fixes

  - Increase query timeout for long running database operations

### 3.516: 06/29/2021

Bug fixes

  - ESRI integration no longer creates services
  - FTP download does not work
  - Remove Android APK - use the one on the store

### 3.515: 11/15/2020

Bug fixes

  - Notebook use can crash when used with global values
  - FTP can create blank files

### 3.514: 04/21/2020

Bug fixes

  - Send as email attachment does not work properly

### 3.508: 8/22/2019

Bug fixes

  - Web Update doesn't create folder on OneDrive backed up desktops

### 3.507: 7/7/2019

Bug fixes

  - Web list doesn't clear if response is empty

### 3.505: 5/29/2019

Bug fixes

  - Crash on Android 9 when using GPS to set the time

### 3.504: 5/18/2019

Bug fixes

  - Crash when attaching images to alerts

### 3.503: 5/15/2019

New features:

  - Client setting to defer updates unless on WiFi network

Bug fixes:

  - ESRI Connect stopped working when TLS 1.2 was made a requirement (by
    ESRI)

### 3.501: 3/10/2019

Bug fixes:

  - Workaround for compiler bug in new tooling
  - Auto send timeout should be in seconds, not minutes

### 3.500: 3/4/2019

Bug fixes:

  - Fix to work on older Android devices (down to KitKat)

### 3.499: 1/10/2019

Bug fixes:

  - Fix to work on older Android devices (down to KitKat)

### 3.498: 1/1/2019

Bug fixes:

  - Attempt to get data from all connected devices

### 3.497: 12/28/2018

Bug fixes:

  - Time offset not saved between resets

### 3.496: 12/03/2018

Bug fixes:

  - Camera crashes

### 3.494: 12/01/2018

Bug fixes:

  - Phone number control doesn't always work
  - Foreground service sometimes crashes the app

### 3.491: 11/25/2018

Bug fixes:

  - On Android Oreo, activate a foreground service to keep CyberTracker
    alive when a track timer is active

### 3.490: 10/07/2018

Bug fixes:

  - ESRI upload should not use CyberTracker ids

New features:

  - Element Phone number: retrieve the device phone number

### 3.489: 08/26/2018

Bug fixes:

  - ESRI upload fails on Android
  - Some devices are not recognized

### 3.486: 06/23/2018

Bug fixes:

  - Random crash on latest Android phones

### 3.482: 04/22/2018

Bug fixes:

  - Never send duplicate data, except for edit scenario
  - Don't process update requests less than 1 minute apart

### 3.479: 03/25/2018

Bug fixes:

  - Some devices are not recognized

### 3.478: 03/16/2018

Bug fixes:

  - Distance calculation should use speed instead of location
  - Remove Looped Attributes Action doesn't work for check and number
    lists

### 3.476: 12/28/2017

Rebuilt to ensure a good build

### 3.474: 12/02/2017

Bug fixes:

  - Distance calculations don't always work on Android
  - Android time resolution was sub 1s - this needs to be rounded
  - Element web list incorrectly handled tab character
  - OTA servicing sends corrupt data when the "Clear after send" is
    unchecked
  - Logging for HTTP requests
  - Export to external database did not handle doubles correctly

New features:

  - "Output as time" from ElementFormula

### 3.466: 11/05/2017

Bug fixes:

  - Timer track breaks causes CT\_TOTAL\_DISTANCE to reset
  - Simple camera sometimes doesn't autofocus

### 3.465: 10/08/2017

Bug fixes:

  - Bug with new CT\_TOTAL\_DISTANCE formula, doesn't work with write
    track break

### 3.464: 10/08/2017

Bug fixes:

  - Bug with new CT\_TOTAL\_DISTANCE formula

### 3.463: 10/03/2017

Bug fixes:

  - Parse error when too looking at the map and there are too many
    fields
  - ESRI plugin fixed

### 3.462: 10/01/2017

Bug fixes:

  - Web List should update less frequently

New features:

  - New global value "CT\_TOTAL\_DISTANCE" which can be used in formulas
  - Can pass a link to users in email that will automatically trigger
    Install From Web feature

### 3.461: 09/26/2017

Bug fixes:

  - Error when saving to DropBox

### 3.460: 09/23/2017

Bug fixes:

  - Web update sometimes updates multiple times
  - URL on Web Update should default to "http"
  - Element Panel can accept text that contains tabs
  - Element Web List can accept text that contains tabs
  - Element Panel fails to track Elements properly if output type is
    Value

### 3.459: 09/09/2017

Bug fixes:

  - Web update error messages should be human readable
  - Persist the URL on the Install From Web dialog

### 3.455: 08/30/2017

New features:

  - Web update should have a custom string that can be used in the app

### 3.454: 08/22/2017

Bug fixes:

  - FTP should default to passive mode

### 3.453: 08/20/2017

New features:

  - Add attribute action has more kinds of Ids that it can emit.

### 3.452: 08/13/2017

Bug fixes:

  - Improvements to automatic update feature

### 3.451: 08/01/2017

Bug fixes:

  - Kiosk mode sometimes causes track timer to fail on Android

### 3.450: 07/24/2017

Bug fixes:

  - Windows Mobile client broken

### 3.449: 07/16/2017

New features:

  - New Action: Remove Looped Attributes

### 3.448: 07/12/2017

Bug fixes:

  - SD card insert crashes CyberTracker - should just close the current
    app

New features:

  - GeoJSON upload uses Element IDs rather than text name
  - New control Element Web List provides list contents that can be
    downloaded from the web
  - Web Update feature which allows application updates over the web

### 3.445: 06/09/2017

New features:

  - ESRI shape file export should choose field types correctly
  - Snap GPS not blocking correctly, prevents correct time coming from
    GPS

### 3.443: 03/28/2017

New features:

  - Bug fix for ESRI online feature
  - Video for ESRI online feature

### 3.442: 03/06/2017

New features:

  - ESRI online feature supports attachments

### 3.441: 12/18/2016

Bug fixes:

  - Remove critical battery level check that disables timer tracks: OS
    will manage this
  - Improve Android GPS state mechanism
  - Timer track point is now emitted with a sighting if the track log is
    turned on
  - Waypoint engine assert errors on desktop are removed

New features:

  - Android settings lets user enter a user name override

### 3.440: 09/24/2016

Bug fixes:

  - Changes to get SD backup working on more devices

### 3.438: 09/18/2016

Bug fixes:

  - Changes to get SD backup working on more devices

### 3.437: 09/17/2016

Bug fixes:

  - SD card backup for Android

New features:

  - Add more math functions to the parser: sin, cos, tan, ceil, floor,
    log, sqrt, etc.
  - New Action: Transfer on Save

### 3.436: 09/16/2016

Bug fixes:

  - Error message regarding SD card too small even when not using SD
    card for backups

### 3.435: 09/11/2016

Bug fixes:

  - Improvements and fixes to the JSON send and Alert mechanism

New features:

  - ESRI ArcGIS online connection

### 3.426: 08/05/2016

Bug fixes:

  - FTP protocols should default to binary mode
  - Android JSON has a trailing byte

### 3.425: 08/05/2016

Bug fixes:

  - Streamlining CTX and JSON file creation and sending
  - Download and send JSON files from the desktop if they fail to send
    on the device

### 3.423: 07/30/2016

Bug fixes:

  - Track files don't reset on Windows Mobile
  - Error messages may show on Windows Mobile after uploading an image

### 3.422: 07/25/2016

Bug fixes:

  - CTX export broken
  - Improvements to JSON export
  - Upload of JSON from desktop does not work

### 3.418: 07/13/2016

Bug fixes:

  - Tweaks to JSON protocol
  - ESRI JSON support

### 3.417: 07/13/2016

Bug fixes:

  - JSON upload doesn't use HTTPS on Desktop
  - CreateCTX from directory doesn't include globals

### 3.415: 07/12/2016

Bug fixes:

  - Image resolution should restrict file size for Element Camera
    control

### 3.414: 07/09/2016

Bug fixes:

  - Crash when deleting sightings and map view visible
  - Non Virtual Earth maps do not export to Field Map with layer data
    correctly
  - Compressed GeoJSON does not upload on Android
  - Images and sounds sent via GeoJSON are corrupt if too large

### 3.412: 05/28/2016

Bug fixes:

  - GeoJSON format fixes and changes

### 3.411: 05/24/2016

Bug fixes:

  - Json export contains bad comma
  - Json time format not the same as w3c format

### 3.410: 05/22/2016

Bug fixes:

  - Json export tweaks: new fields dbName and appName
  - Json time format now includes time zone

### 3.408: 05/14/2016

Bug fixes:

  - Json export not compliant
  - UTC date time doesn't correct for daylight savings
  - Crash with corrupt shape layer on map
  - Windows Mobile app doesn't always install

### 3.404: 04/24/2016

Bug fixes:

  - SnapLastGPS action doesn't work on the screen with the save button
  - Application list should be sorted (fixed on Android only)
  - Keypad that quits application should auto-quit if kiosk mode is not
    active
  - About dialog on desktop has broken link

### 3.403: 03/06/2016

Bug fixes:

  - Crash in kiosk mode

### 3.399: 02/07/2016

Bug fixes:

  - CyberTracker does not work on Android Marshmallow

### 3.398: 01/30/2016

Bug fixes:

  - Crash during mixed Alerts and Transfer

### 3.397: 01/24/2016

Bug fixes:

  - FTP transfer doesn't work on Android

New features:

  - HTTP JSON prototype

### 3.396: 01/20/2016

Bug fixes:

  - FTP transfer doesn't clean up properly

### 3.395: 01/20/2016

Bug fixes:

  - Field maps always have history tracks, even if disabled
  - Disable editing should still allow viewing of past sightings
  - Installing on Windows Mobile devices sometimes doesn't work if
    CyberTracker is already installed

New features:

  - Alerts prototype

### 3.393: 11/17/2015

Bug fixes:

  - Crash during sighting download creates lost data scenario

### 3.392: 11/13/2015

Bug fixes:

  - Kiosk mode fails on some devices
  - Crash using the camera on Android
  - Crash during sighting download

### 3.391: 11/09/2015

New features:

  - Improvements GPS outlier detection in the field

### 3.390: 09/06/2015

Bug fixes:

  - Increase the minimum size of a scroll thumb
  - Persistent scroll location for goto lists
  - Option to disable the compass for use in heading on Android

New features

  - "Text mode" on Element Keypad control

### 3.389: 08/09/2015

Bug fixes:

  - Automatically recover corrupt sightings
  - Retargeted scenario additional GPS info for debugging outliers

### 3.388: 07/27/2015

Bug fixes:

  - Do not use Orphans for missing re-targeted CTX files

### 3.387: 07/16/2015

Bug fixes:

  - Improvements to Kiosk mode on Android

New features:

  - "/OneOnly" command-line option for testing

### 3.386: 06/14/2015

Bug fixes:

  - Improved logging on download sighting path
  - Improvements to Kiosk mode on Android
  - Improvements to external front end support

### 3.385: 06/07/2015

Bug fixes:

  - Crash on Android version 5
  - Database download failure on Android when doing a sync multiple
    times without closing the application

### 3.384: 05/25/2015

New features:

  - Improved Kiosk mode for Android
  - Ability to set sample rate for audio recorder via the "Sample rate"
    property

Bug fixes:

  - Improved audio recording on Android
  - Incorrect handling of comma in certain locales lead to bad paths
  - Snap Date and Time Action should turn on the GPS if system requests
    GPS time to be in sync
  - Skip should save state of current screen

### 3.382: 04/19/2015

New features:

  - "Scale for touch" property for list controls to allow override of
    touch mode

Bug fixes:

  - Improved audio recording on Android
  - Snap date and time should not snap without GPS if "Use GPS time" is
    set

### 3.381: 02/03/2015

New features:

  - Support for PostgreSQL

Bug fixes:

  - Crash reading large databases

### 3.380: 01/31/2015

New features:

  - Support for PostgreSQL

Bug fixes:

  - Crash exporting large databases

### 3.376: 01/19/2015

Bug fixes:

  - Time can be wrong on Android devices
  - Problem upgrading from 3.374

### 3.375: 01/12/2015

Bug fixes:

  - New certificate signing doesn't work on Windows Mobile

### 3.374: 01/10/2015

New features:

  - Date control tweaks
  - Aerial transect tweaks
  - Resilience for corrupt sightings

### 3.373: 01/07/2015

New features:

  - Date control
  - New digital certificate: must uninstall old version on Android

### 3.372: 11/22/2014

Bug fixes:

  - Use GPS for time doesn't work on Android
  - User lists don't work for non-standard characters
  - Improvements to the Bulk Edit Sightings Transect tab

### 3.371: 10/26/2014

Bug fixes:

  - Flint device doesn't take pictures in Kiosk mode
  - Control state not preserved in Scrollbox controls

### 3.370: 09/29/2014

New features:

  - Special return codes for command line tool when downloading

### 3.369: 09/21/2014

New features:

  - Creating a new map view should center on sightings
  - Inclination should be taken into account when computing transects

Bug fixes:

  - Element Formula control needs text descriptions for properties

### 3.368: 09/02/2014

Bug fixes:

  - Basic mode should allow screen names not to be edited
  - User lists should be resilient to blank lines
  - User lists show a blank box after names on Windows Mobile devices

### 3.367: 08/24/2014

New features:

  - Basic mode for limited editing of applications (under password
    protection)
  - User lists: editable lists that will not corrupt the application

### 3.366: 08/05/2014

New features:

  - Element Lookup List in Beta - add auto next

Bug fixes:

  - Client - Crash when using Element Panel with Value field

### 3.365: 08/04/2014

New features:

  - Element Lookup List in Beta

### 3.364: 07/29/2014

Bug fixes:

  - Client - Alignment failure when changing profiles with bottom docked
    controls that are autosized
  - Client - Failed to block next from field map when Element list on
    screen allows next

### 3.363: 07/17/2014

Bug fixes:

  - Desktop - Date filtering for timer tracks fails for non-US date
    ranges

### 3.362: 07/06/2014

New features:

  - Desktop: new icons

Bug fixes:

  - Desktop - High DPI improvements
  - Desktop - Native support for Windows \* 1

### 3.361: 07/05/2014

New features:

  - Desktop: new icons

Bug fixes:

  - Client: Incorrect Element selected from auto-select-index on
    filtered lists

### 3.360: 07/02/2014

New features:

  - Desktop: new icons

Bug fixes:

  - Client: Crash with offscreen sorted Element Lists

### 3.359: 06/29/2014

New features:

  - Desktop: new icons

### 3.358: 06/28/2014

New features:

  - Client: Improvements to simplified camera on Android

### 3.357: 06/24/2014

New features:

  - Client: Improvements to simplified camera on Android

### 3.356: 06/22/2014

New features:

  - Client: Simplified camera on Android

### 3.355: 06/15/2014

Bug fixes:

  - Desktop: Fix cannot set view issue with multiple field maps
  - Desktop: SD backup on desktop broken

### 3.354: 06/06/2014

Bug fixes:

  - Desktop: Error message when exporting shape files with duplicate
    column names
  - Desktop: Crash on map when using columns names containing the quote
    character

### 3.353: 05/22/2014

Bug fixes:

  - Client: Crash when using timer on Android devices
  - Client: Crash when using bluetooth headset on Android devices
  - Client: Field map inspector doesn't have sound playing feature
  - Desktop: Class breaks legend doesn't display correctly for ranges

### 3.352: 05/17/2014

Bug fixes:

  - Client: Crash when field maps deleted from file system
  - Client: State key reset not working on text editor
  - Client: Field maps should not show view errors with no GPS fix
  - Desktop: Double entries shown in Frequency graph when deleting
    sightings
  - Desktop: Crash with certain characters in shape file field names
  - Desktop: Grid renderer legend doesn't work when too many cells are
    shown

### 3.350: 05/08/2014

Bug fixes:

  - Desktop: Fail when merging CTX files with media
  - Desktop: Crash when deleting map that was referenced

New features:

  - Improved legend on field map

### 3.349: 04/24/2014

New features:

  - Retain state feature on Element Text Edit controls
  - Notes can be added to a screen in layout mode
  - Trend graphs now have 8 series

### 3.348: 04/16/2014

Bug fixes:

  - Client: Field maps should persist zoom setting
  - Desktop: Crash when loading bad data file
  - Android: GPS timer doesn't resume during rotation or other focus
    lost events

New features:

  - Field maps support a friendly name
  - Field maps support a Group which can be used to filter groups of
    maps

<!-- end list -->

  - 347: 04/05/2014 ===

New features:

  - Desktop and client: Multiple moving maps

### 3.346: 03/18/2014

Bug fixes:

  - Desktop: Hang painting default map (not Virtual Earth)

### 3.345: 03/15/2014

Bug fixes:

  - Desktop: Layers don't respect the color properly

### 3.344: 03/09/2014

Bug fixes:

  - Desktop: When creating a CTX from predefined application, startup
    mode should be Applications
  - Desktop: Field map on skip should be under GPS settings on a
    per-application
  - Desktop: GPS Simulator should auto-set the center location
  - Desktop: UTM ECW maps created outside CyberTracker should be
    auto-detected
  - Client: Notebook control buttons don't work if not left aligned

New features:

  - Client: Filter text after for Bar code control

### 3.343: 03/01/2014

New features:

  - Client: Sounds can be played back from prior sightings

### 3.342: 02/28/2014

New features:

  - BREAKING CHANGE: Desktop: Move all path settings under Database
    Properties
  - Client: History tracks

Bug fixes:

  - Desktop: Exporting a shape file with a DeviceId column fails

### 3.341: 02/26/2014

New features:

  - Desktop: Class breaks can show labels

Bug fixes:

  - Desktop: Legend for grid mode not rendering correctly
  - Desktop: Path color changing not supported for point rendering
  - Desktop: Opening CTX should respect startup mode
  - Client: Forcing user to unplug device even when only charging

### 3.340: 02/20/2014

New features:

  - Desktop: Ability to change track color

Bug fixes:

  - Desktop: Tweaks to class breaks rendering

### 3.339: 02/19/2014

Bug fixes:

  - Desktop: New sightings doesn't work, problems using Layout

### 3.338: 02/17/2014

Bug fixes:

  - Desktop: Labels on sightings causes hang
  - Client: Touch doesn't work on Windows 8

### 3.337: 02/15/2014

New features:

  - Desktop: Label drawing for query layers
  - Client: RangeFinder should be able to snap date, time and GPS along
    with range
  - Client: Font size for text editor should use the size specified in
    the edit control
  - Client: Battery should show if it is charging

Bug fixes:

  - Desktop: Improvements to class breaks system
  - Client: Snap date and time should work even if date and time are not
    specified

### 3.336: 02/02/2014

New features:

  - Desktop: Class breaks rendering for shape file layers

### 3.335: 01/19/2014

New features:

  - Desktop: Expose Element Barcode control in screen templates
  - Client: Element Panel should support output of value

Bug fixes:

  - Client: Images are constrained to 512x512, which is too low for
    modern devices
  - Client: Goto and History do not respect special characters correctly

### 3.334: 01/12/2014

New features:

  - Client: Element Barcode control for scanning barcodes on Android

Bug fixes:

  - Client: Accuracy may be more than 50 on Android devices

### 3.333: 01/07/2014

New features:

  - Desktop: Merging and titling of measure shape files

Bug fixes:

  - Desktop: Memory leak when building map layers
  - Client: Right to left text may not display on Android

### 3.332: 12/28/2013

New features:

  - Desktop: Copy to clipboard for Graphs

Bug fixes:

  - Client: Scaling inside notebook pages doesn't work
  - Client: ScrollBox scroll bar doesn't update properly
  - Desktop: Crash when exporting shape files fails

### 3.331: 12/16/2013

New features:

  - Desktop: Partial day filtering of timer tracks

Bug fixes:

  - Desktop: Crash while loading databases with keypad screens

### 3.330: 12/15/2013

Bug fixes:

  - Client: Scaling factors cause line doubling
  - Client: Crash on Android when deleting last application

### 3.329: 12/13/2013

New features:

  - Desktop and client: Can specify map colors

Bug fixes:

  - Desktop: Field maps should have scale
  - Desktop: Layout mode controls don't size correctly

### 3.328: 12/09/2013

New features:

  - Desktop: Map has north arrow and scale

Bug fixes:

  - Desktop: Hang when creating field map
  - Desktop: Cosmetic fixes to UI
  - Desktop: Console application doesn't work

### 3.327: 12/05/2013

New features:

  - Client: Element List now has an Auto height property

Bug fixes:

  - Client: Crash using Android emulator
  - Client: Cosmetic fixes to UI

### 3.326: 12/04/2013

Bug fixes:

  - Desktop: Crash reading corrupt database
  - Desktop: Exporting to Excel leaves numbers in text format

### 3.325: 12/03/2013

New features:

  - Desktop: Exporting CSV and TSV will alter the filename of the image
    if the column title starts with MEDIA\_
  - Client: Changing between goto points now requires a specific button
    click

Bug fixes:

  - Desktop: Graph view paths were not correctly calculated
  - Client: Bluetooth GPS support accidentally required Android \* 3

### 3.324: 12/01/2013

Bug fixes:

  - Desktop: Crash when failing to connect to Android device
  - Client: Android client crashes during race when GPS is disconnected
  - Client: Goto pointer out of bounds on some screens
  - Client: Bluetooth GPS that does not provide satellite data should
    still be able to provide a fix
  - Client: Crash when downloading strangely corrupt sightings and
    waypoints

### 3.323: 11/29/2013

New features:

  - Client: Should show if re-install is required

Bug fixes:

  - Desktop: Editing static text elements shows bad characters
  - Client: Android client crashes on some older devices with a resource
    error
  - Client: Android client crashes on some older devices without
    Bluetooth headset support
  - Client: Android does not render right aligned text correctly
  - Client: Android Compass jumps around a lot

### 3.322: 11/25/2013

Bug fixes:

  - Client: Android client doesn't install on some devices

### 3.321: 11/24/2013

Bug fixes:

  - Client: RangeFinder and Element Serial can use "Show port state"
    property for testing
  - Client: FTP on android leaking memory
  - Client: Inspector and history don't work together correctly
  - Desktop: Reading non-ascii characters caused issue uploading data

### 3.320: 11/05/2013

Bug fixes:

  - Client: RangeFinder not correctly picking up global values
  - Client: opendir leaking directory handles on Android
  - Desktop: ReplaceText should also replace Elements

### 3.319: 11/03/2013

New features:

  - Client: RangeFinder COM port should be configurable using COM Port
    List control
  - Desktop: Find and Replace for text strings using Bulk Sightings Edit

Bug fixes:

  - Client: COM Port List should not allow Detect to be specified
  - Client: Kiosk mode for Android improvements
  - Desktop: ExportMedia registry key incorrect due to bad config file

### 3.318: 10/13/2013

Bug fixes:

  - Client: Failure to show history when only one entry
  - Client: History does not show extended characters
  - Client: Element List does not add links correctly for number lists
    with checks

### 3.317: 09/20/2013

Bug fixes:

  - Client: Android less than 4 install broken

### 3.316: 09/19/2013

New features:

  - Client: Android support for Bluetooth headsets for sound record and
    playback

Bug fixes:

  - Desktop: Fix for Android \* 3
  - Client: Android should hide the keyboard when pressing Ok button

### 3.315: 08/24/2013

Bug fixes:

  - Desktop: New graphic for Help About
  - Desktop: New links in Help menu
  - Desktop: New telemetry system
  - Desktop: Minor changes to screen templates and samples
  - Client: Improvements for non-English support

### 3.311: 08/18/2013

New features:

  - Desktop: Additional simplified templates

Bug fixes:

  - Desktop: Export shape file doesn't work if column has multiple
    numbers
  - Desktop: ExportMedia path should be published in the registry
  - Desktop: Changing the screen name in the central panel doesn't work
  - Desktop: Saving is very slow when using the History feature
  - Client: Improved FTP support
  - Client: Improved synchronization
  - Client: Check list min and max checked fail on filter screens

### 3.310: 08/11/2013

New features:

  - Desktop: CTX files contain database name
  - Desktop: Additional simplified templates

Bug fixes:

  - Desktop: Failed to install maps
  - Desktop: Hang during application install
  - Desktop: Very slow save when using history feature

### 3.309: 07/30/2013

Bug fixes:

  - Client: Android timing crashes from Telemetry
  - Client: Android should display OK button
  - Client: Android audio should take wake lock
  - Desktop: Darwin core export should fill in attribute for null types

### 3.308: 07/21/2013

New features:

  - Desktop: Export Darwin Core XML
  - Desktop: Screen names break on localization
  - Client: GPS reading should not be discarded if valid, but less than
    threshold
  - Client: ElementList min checks and max checks
  - Client: Notebook control sometimes doesn't resize correctly

Bug fixes:

  - Desktop: Statics don't display in drop down
  - Client: Scrollbars too wide in touch mode
  - Client: NumberList column count should always be respected
  - Client: Screen state should always be stored in case of unexpected
    exit
  - Client: ElementList details should show icon if main icon is set

### 3.307: 07/15/2013

New features:

  - Client: Play sound on Android
  - Client: Record sound on Android
  - Client: Camera doesn't work on some Android devices

Bug fixes:

  - Desktop: Tweak uploadpda command line and add support for regkey
    download targets
  - Client: Crash with timers on Android

### 3.306: 07/07/2013

New features:

  - Desktop: Updated screen templates
  - Desktop: Updated screen sizes
  - Desktop: Support for Zoom 50%

Bug fixes:

  - Desktop: Increase default scroll bar width
  - Desktop: Export raw XML fails
  - Desktop: Reduce options for uploadpda command line
  - Desktop: Upload chunk size for WPD
  - Client: Column width scaled incorrectly resulting in too few columns

### 3.305: 07/04/2013

New features:

  - Desktop: Updated screen templates
  - Desktop: Updated screen sizes
  - Desktop: Can specify final CTX directory via command line
  - Desktop: RawXML output should also outpoint timer tracks
  - Desktop: Optimations for reading and exporting large data sets
  - Desktop: Default to World map ECW
  - Client: Android upload to FTP
  - Client: Android timer tracks
  - Client: Random number generation via the Add Attribute action

Bug fixes:

  - Desktop: Ignore deleted sightings when importing data to a change
    free database
  - Desktop: Crash after downloading data
  - Client: Android blue bar sometimes doesn't contain text
  - Client: Numerous tweaks to controls for Android

### 3.304: 06/23/2013

New features:

  - Desktop: New screen templates
  - Client: Improvements to Keypad button spacing

Bug fixes:

  - Desktop: RawXML export should correct export XML special characters
  - Desktop: Crash after downloading data
  - Client: Camera doesn't always capture images

### 3.303: 06/17/2013

New features:

  - Desktop: New screen templates
  - Desktop: Standardize fonts to Arial and Courier

Bug fixes:

  - Client: Carriage returns are not respected on client
  - Client: Change Auto Radio Next to Auto Next
  - Desktop: New sightings doesn't work for temporary databases
  - Desktop: Very large sighting counts causes crash

### 3.302: 06/12/2013

New features:

  - Desktop: New screen templates
  - Desktop: New screen profiles
  - Desktop: Command line to export raw XML
  - Desktop: Command line to upload application to device
  - Desktop: Command line to create a CTX from a directory

Bug fixes:

  - Client: Fail on older PocketPC devices
  - Desktop: Non ECW maps don't export to field map correctly if
    projection is set to Virtual Earth
  - Desktop: Performance improvements for large applications (many
    screens and Elements)

### 3.301: 06/02/2013

New features:

  - Client and Desktop: Touch mode to automatically scale old screens
  - Desktop: RAW XML export contains Elements definitions
  - Desktop: Sound continues playing even if focus changes

Bug fixes:

  - Desktop: Rename Profiles to Sizes
  - Desktop: Crash on download
  - Desktop: Corruption of data on sightings with media (only in ===
    3.300)
  - Client: Fail to upload sightings

### 3.300: 05/27/2013

New features:

  - Client: New control: SightingList
  - Client: Add Interval property to Element Number control
  - Desktop: Export RAW XML
  - Desktop: Changes to query table should not clear filter
  - Desktop: Frequency graph should use count of Element if possible

Bug fixes:

  - Client and Desktop: Support for multiple languages across Android
    and Windows
  - Desktop: Move Get data from device under the File menu from the
    Tools menu
  - Desktop: Failure when importing very large databases
  - Desktop: When syncrhonizing application to device, sometimes
    application does not launch
  - Client: Titlebar doesn't work unless at the top of the screen
  - Client: Goto doesn't show targets correctly
  - Client: ElementList crashes on details mode if too small

### 3.298: 04/16/2013

Bug fixes:

  - Desktop: Map status display not working

### 3.296: 03/26/2013

New features:

  - Client: Add EXP() and POW() to Element Formula control
  - Client: Add Interval property to Element Number control

Bug fixes:

  - Desktop: Uploading via MTP very slow if multiple Applications
    already installed

### 3.295: 01/19/2013

New features:

  - Client: Auto height property for Panels.

Bug fixes:

  - Client: Android should support extended characters.

### 3.294: 01/14/2013

New features:

  - Desktop + Client: Android support.
  - Desktop: Font scaling.
  - Desktop: New screen sizes.
  - Desktop: Installing Android APK to device.
  - Desktop: Fixed new logo sizes.
  - Client: Bring back support for older PocketPC devices.

Bug fixes:

  - Client: Crash when editing is disabled.

### 3.292: 12/24/2012

New features:

  - Desktop: DeviceId column in query table.
  - Desktop: Signing of MSI and Windows Mobile CAB.
  - Desktop: Support for High DPI desktop displays and font scaling.
  - Desktop: Added new logo.
  - Desktop: Support for Portable Media Device syncing.

Bug fixes:

  - Desktop: New Element should associate the Element with the current
    category.
  - Desktop: System font scaling should not change client font sizes.
  - Client: Sighting ids should be combined with device ids to improve
    uniqueness.

### 3.291: 11/21/2012

Bug fixes:

  - Desktop: Provide a way to turn off system fonts to get exact font
    sizing.

### 3.290: 11/04/2012

Bug fixes:

  - Client: Ampersands not ignored when drawing text.
  - Desktop: Database corruption can cause images to be unexportable.

### 3.289: 10/28/2012

Bug fixes:

  - Client: Font rendering issue.

### 3.288: 10/28/2012

Bug fixes:

  - Client: Memory leak using multiple fonts.

### 3.287: 10/28/2012

Bug fixes:

  - Client: Camera doesn't always work on Juno devices at 5MP.
  - Client: Kiosk mode doesn't work properly with camera.
  - Client: Special fonts should be transferred to device.

### 3.286: 10/21/2012

Bug fixes:

  - Client: Installing to Windows Mobile fails when application doesn't
    already exist.
  - Client: Camera doesn't allways work on Juno devices.
  - Client: Kiosk mode can be bypassed on some devices.

### 3.285: 09/16/2012

New features:

  - Desktop: Upload applications and download data from Android devices.
    Testing only.

### 3.284: 08/26/2012

Bug fixes:

  - Client: Memory leaks when using map cause application to crash.

### 3.283: 07/17/2012

New features:

  - Desktop: Switch to desktop button on New Sightings dialog.

Bug fixes:

  - Client: State not stored when pressing back on retain state.
  - Client: Reset state key needs to be able to delay until save.

### 3.282: 07/03/2012

Bug fixes:

  - Client: Produce error if saving to SD card fails.

### 3.281: 06/17/2012

Bug fixes:

  - Client: Rework database to allow for large sighting counts.

### 3.280: 06/11/2012

Bug fixes:

  - Desktop: Altitude sometimes not editable.
  - Client: Crash when using title bar and big fonts.
  - Client: Lost Options setting.

### 3.279: 06/02/2012

Bug fixes:

  - Desktop: Improve robustness of saving.
  - Client: Improve database size by ignoring default properties.
  - Client: Minor changes to UTM co-ordinates.

### 3.278: 05/28/2012

Bug fixes:

  - Desktop: Fix bad build.

### 3.277: 05/27/2012

New features:

  - Desktop: Bulk edit-Add should allow statics and skip existing.
  - Client: Support for UTM co-ordinates on GPS and sighting edit
    screens.

Bug fixes:

  - Desktop: More memory efficient reader for CTX files.

### 3.275: 03/27/2012

Bug fixes:

  - Desktop: Path calculations broken with recent change.

### 3.274: 03/23/2012

Bug fixes:

  - Desktop: Range attributes for Element RangeFinder are not
    changeable.

### 3.273: 03/18/2012

Bug fixes:

  - Desktop: Minor improvements to optimization.

### 3.272: 03/18/2012

New features:

  - Desktop: Optimized save and load performance.

Bug fixes:

  - Desktop: Selectable range attributes in bulk transect edit.
  - Client: Range attributes for Element RangeFinder are not changeable.
  - Client: Support for Windows Mobile \* \*

### 3.271: 03/04/2012

Bug fixes:

  - Desktop + Client: External databases should not require local
    versions for each computer.
  - Client: Robustness improvements for serial communications.

### 3.270: 02/09/2012

Bug fixes:

  - Desktop: Show hectares and acres for map view area calculations.
  - Client: Compass should have NSEW text around it.
  - Client: GPS control should have Heading style.

### 3.269: 01/20/2012

Bug fixes:

  - Desktop: Efficiency graph only uses paths with sightings to compute
    total distance and time.
  - Desktop: Paste sightings from Excel should use system date format.

### 3.268: 11/26/2011

New features:

  - Client: Compass control.

Bug fixes:

  - Client: Loops containing images and sounds are not cleared
    correctly.

### 3.267: 11/12/2011

New features:

  - Desktop: Area computation and creation of shape files.

Bug fixes:

  - Desktop: Pasting media doesn't save correctly.

### 3.266: 10/23/2011

Bug fixes:

  - Client: Elements don't show up on Field Map.
  - Desktop: Bad sighting created by Paste New sightings.
  - Desktop: Crash when changing properties.
  - Desktop: Palm doesn't show Goto point distance correctly.

### 3.265: 10/02/2011

Bug fixes:

  - Client: SD card backup doesn't always work.
  - Desktop: Reduce crashes when running out of system resources.
  - Desktop: Tag output should be redirected when attribute result is
    Element.
  - Desktop: Remove hard errors.

### 3.264: 09/18/2011

Bug fixes:

  - Client: RangeFinder needs a Keep connected option to prevent long
    delays when working with serial devices.
  - Desktop: Paths should be expanded in case they contain environment
    variables.

### 3.263: 08/29/2011

Bug fixes:

  - Client: Element Serial data needs a Keep connected option to prevent
    long delays when working with serial devices.

### 3.262: 08/25/2011

Bug fixes:

  - Desktop: Save of data CTX deletes data.
  - Desktop: Using an ampersand in a file name makes New Sightings
    feature not work.
  - Desktop: Using UNC transfer does not work with New Sightings
    feature.

### 3.261: 08/09/2011

New features:

  - Client: Field Map can use Inspector selection to set current GPS
    position.

Bug fixes:

  - Client: Some GPS devices do not work.

### 3.260: 08/05/2011

Bug fixes:

  - Client: Crash when using Skip GPS.
  - Client: Soft keyboard sometimes displays over screen.
  - Desktop: History should be updated whenever a connection is made.
  - Desktop: Aerial transect settings do not work properly.

### 3.259: 08/01/2011

Bug fixes:

  - Desktop: Occasional runtime crash due to corrupt compiler settings.

### 3.258: 07/31/2011

New features:

  - Client: Elements are visible on field map.
  - Client: Map Inspector can set Goto target.
  - Client: Element Serial control can parse input into Elements.
  - Client: Element Serial control can send data to a device.
  - Desktop: Aerial Survey transect calculations via Bulk Edit.

Bug fixes:

  - Client: Number list fast tap should not work when check is not
    enabled.
  - Client: Maximum Element Recorder button width too small.
  - Desktop: Occasional hang when using the Element Serial control.
  - Desktop: Pasting Elements with blank names causes crash.

### 3.257: 06/30/2011

Bug fixes:

  - Desktop: Paste from Excel should work for Latitude and Longitude
    fields.

### 3.256: 06/27/2011

Bug fixes:

  - Client: Element list doesn't add result to sighting.

### 3.255: 06/26/2011

New features:

  - Desktop and Client: Elements can have Latitude and Longitude and set
    current Goto target.
  - Client: More properties to control points on Field Map.

### 3.254: 06/17/2011

Bug fixes:

  - Desktop: UseSD backup on desktop feature causes error messages for
    some kinds of removable drives.
  - Desktop: UseSD backup feature doesn't clean up properly.
  - Desktop: UseSD backup feature close button still asks for cancel.

### 3.253: 06/14/2011

Bug fixes:

  - Desktop: UseSD backup on desktop feature causes error messages if no
    CyberTrackerData directory found.

### 3.252: 06/05/2011

Bug fixes:

  - Desktop: Complete UseSD backup on desktop feature.

### 3.251: 06/02/2011

Bug fixes:

  - Desktop: CS01 failed to upload applications.

### 3.250: 06/01/2011

Bug fixes:

  - Client: Crash when using Field Map Inspector.

### 3.249: 05/28/2011

Bug fixes:

  - Client: Crash when adding point data from map to sighting.

### 3.248: 05/25/2011

Bug fixes:

  - Desktop: Non VE field maps do not have correct view.
  - Desktop: SQL export does not export images correctly.
  - Client: Windows Mobile \* 5 support.
  - Client: CAB creation on client generates wrong checksum on CTX
    files.
  - Client: CAB creation may corrupt image files.
  - Client: Lists should clear prior data if no new selection is made.

### 3.247: 05/22/2011

Bug fixes:

  - Desktop: Map datums not always respected.
  - Desktop: Crash when writing to log file.
  - Desktop: Elements should be shown in sorted order.
  - Client: 2400 baud should be supported.
  - Client: GPS time sync incorrect for some time zones.

New features:

  - Desktop: Rework New sightings.
  - Desktop and Client: Rework Field Map support.

### 3.246: 04/25/2011

Bug fixes:

  - Desktop: History should not export deleted sightings.
  - Desktop: Field map creation should be sized according to the view
    window.

### 3.245: 04/22/2011

Bug fixes:

  - Client: Number lists with keypad cannot be edited.
  - Desktop: Login prompt appears for databases without username and
    password.

New features:

  - Client: Number list checks property for number lists.

### 3.244: 04/17/2011

New features:

  - Client: Expose History and Map Inspectors as controls.
  - Desktop: Add tools option to enable automatic downloading for per
    user installs.
  - Desktop: Per user installation.

### 3.243: 04/15/2011

Bug fixes:

  - Client: Crash when placing flag on Field Map.

New features:

  - Desktop: Last segment length displayed when using measure.

### 3.242: 04/06/2011

Bug fixes:

  - Client: RangeFinder control should use skip instead of jump.
  - Desktop: Improve robustness of corrupt sighting handling.

New features:

  - Client: Map Inspect.
  - Desktop: Include path time in transect calculations.

### 3.241: 03/24/2011

Bug fixes:

  - Client: RangeFinder control crashes when Next screen is set.

### 3.240: 03/20/2011

Bug fixes:

  - Desktop: Perpendicular distance should not be added as near zero.
  - Client: RangeFinder should not snap if Jump screen set and next is
    pressed.

### 3.239: 03/14/2011

Bug fixes:

  - Desktop: Pasting filters should clear existing filter.
  - Desktop: Perpendicular distance should not be added as near zero.
  - Client: Sorted property of Element List should sort Aliases.

New features:

  - Desktop: Simple history.

### 3.238: 02/12/2011

Bug fixes:

  - Desktop: Outgoing files should be processed most recent first.
  - Desktop: Perpendicular distance should not be added as zero.
  - Client: Field map zoom should be 20% at a time.
  - Client and Desktop: FTP download and upload should handle
    differences in FTP protocols.
  - Client: SnapTime, SnapGPS and SnapLastGPS do not work correctly when
    editing existing sightings.
  - Client: Com Port select control should allow default setting.

New features:

  - Desktop: Staging files that fail to upload are moved to the Orphans
    folder.

### 3.237: 01/16/2011

Bug fixes:

  - Desktop: Paste sightings should check for duplicate sightings.
  - Desktop: Paste sightings should mark sightings as having been
    pasted.

\=== 3.Transect: Sightings should be marked according to whether or not
they will be in the transect.

### 3.236: 01/09/2011

Bug fixes:

  - Client: Crash when using camera on Nautiz devices.

New features:

  - Desktop: Paste new sightings from Excel.
  - Desktop: Transect move points.

### 3.235: 12/30/2010

Bug fixes:

  - Desktop: Virtual earth map location incorrectly detected.
  - Client: Auto-next for Element RangeFinder should use Jump instead of
    Next.
  - Client: Navigator back and next button controls should respond to
    Next and Back keypresses.

New features:

  - Client: Keypad formula mode property for Element Lists using Number
    keypad list mode.

### 3.234: 12/08/2010

Bug fixes:

  - Client: Keypad on formula mode presses = if needed before advancing.
  - Client: Crash when using camera.
  - Desktop: Improper date handling for non-US dates.

### 3.233: 11/28/2010

Bug fixes:

  - Client: Purge COM port buffers on connect.

### 3.232: 11/28/2010

Bug fixes:

  - Client: Multiple serial range finders cause asserts to fire.

New features:

  - Client: Element List History sort mode.

### 3.231: 11/27/2010

Bug fixes:

  - Client: Multiple serial devices cause crashes.
  - Client: Sound recording should fail over to sample rate for slower
    devices like BT headsets.
  - Desktop: Entering dates is broken for countries with day-month-year
    formats.

### 3.230: 11/26/2010

New features:

  - Client: Element RangeFinder can set COM port and add an Element on
    success.
  - Client: Element Keypad has a new property: Require set value.

### 3.229: 11/08/2010

Bug fixes:

  - Client: Baud rate selection required for Com Port List control.

New features:

  - Client: Element RangeFinder now as Next screen property.

### 3.228: 11/07/2010

Bug fixes:

  - Client: Element serial does not respect Show port select button.
  - Client: Show 20 serial ports on desktop.

New features:

  - Client: Allow changing of serial port for GPS and RangeFinder.

### 3.227: 10/31/2010

Bug fixes:

  - Desktop: Fails to download track points correctly. === 3.226 voided.

### 3.226: 10/31/2010

Bug fixes:

  - Client: GPS control should display zone corrected time.
  - Client: Sound recorder should pick default recording device.
  - Client: Field map track thickness should scale with the screen
    resolution.
  - Desktop: Correct date and time external database output formats.

New features:

  - Client: Improve display of field map pointer.
  - Client: Action to break timer tracks.
  - Client: Required property for Element Camera.

### 3.225: 10/19/2010

New features:

  - Client: Sending of images and sounds from device is less memory
    intensive.

### 3.224: 10/17/2010

New features:

  - Client: Sending of images and sounds from device now occurs.
  - Desktop: Exception handling for command line database export.
  - Desktop: Improved date and time handling for external database
    export.

### 3.223: 09/26/2010

New features:

  - Client: History sorted property on Element List to move already
    selected items to the end of the list.
  - Client: Support for MDL LaserAce RangeFinder.
  - Desktop: Transect Bulk-Edit feature.

### 3.222: 08/29/2010

New features:

  - Client: History mode for Element Lists to show items that have
    previously been selected.
  - Desktop: Database export of image or sound will be exported as a
    blob field.

### 3.221: 07/08/2010

New features:

  - Client: Port can be selected on the PDA for Serial data control.
  - Client: Formula mode for Keypad control allows computation in the
    field.
  - Client: Retain screen state while navigating through the
    application.

### 3.220: 06/25/2010

Bug fixes:

  - Desktop: Increase robustness of handling of corrupt sightings.

### 3.219: 06/20/2010

Bug fixes:

  - Client: Always show "Skip screen" on navigator.

New features:

  - Desktop: Count per time in Frequency graph.

### 3.218: 06/06/2010

Bug fixes:

  - Client: One line text controls allow new lines.

New features:

  - Desktop: Bulk delete of elements from sightings.
  - Desktop: Create new sightings from the desktop.

### 3.217: 05/27/2010

Bug fixes:

  - Client: Performance optimization for Raindance control.

### 3.216: 05/23/2010

New features:

  - Client: Alias override for Element List control.

### 3.215: 05/01/2010

Bug fixes:

  - Desktop: Pick up bug fixes from latest version of UI components.

New features:

  - Client: Element Serial Data: control to read data from a serial or
    bluetooth port.

### 3.214: 04/09/2010

Bug fixes:

  - Desktop: More helpful errors for new key format.
  - Desktop: Exported media files should not create duplicates in the
    ExportedMedia folder.
  - Desktop: Media export failures should be diagnosable.

New features:

  - Desktop: Excel paste of Elements can include file paths for pasting
    media.

### 3.213: 04/04/2010

Bug fixes:

  - Desktop: EDB files should be able to connect to MDB databases.
  - Desktop: Copy and Paste should remove soft deleted objects.
  - Desktop: Improvements and fixes to Google Earth export.
  - Desktop: Column tags do not work for Alias and Text fields.
  - Desktop: EDB files not parsed correctly for user name and password.
  - Desktop: Exported media always go to set location.

New features:

  - Desktop: New key format for Paste from Excel

### 3.212: 03/27/2010

Bug fixes:

  - Client: Crash when using voice recorder with text entry.

New features:

  - Desktop: Export to KMZ (Google Earth format) from Table
  - Desktop: Id System type which can be displayed to uniquely identify
    sightings
  - Desktop: More tags
  - Desktop: Export to TSV (tab separated values)
  - Desktop: Tables can show any Element property, not just Value, name
    and Tag
  - Desktop: Export of collected media data to files via CSV and TSV

### 3.211: 03/14/2010

Bug fixes:

  - Desktop: Occasional crash when merging.
  - Desktop: Grid rendering cell mouse-over event doesn't pick the right
    cell.

New features:

  - Client: Sound recorder confirm delete
  - Client: Sound recorder required option
  - Client: Sound recorder delete if too short
  - Desktop: Shape export of grid will export a grid shape file
  - Desktop: Option to set the size of the timer points
  - Desktop: Logging for download and upload operations
  - Desktop: GeoTagger sample Application

### 3.210: 03/07/2010

Bug fixes:

  - Client: Older PDAs may crash when using the Element container
    control.

### 3.209: 03/07/2010

New features:

  - Client: Improvements to sound recording based on feedback.

### 3.208: 02/28/2010

New features:

  - Client: Sound recording.

### 3.207: 02/17/2010

Bug fixes:

  - Client: Crash when returning from Camera control.
  - Desktop: Last and current fiscal year date ranges don't work
    properly.
  - Desktop: Export of integrated track does not respect projection for
    timer points.
  - Desktop: Crash when setting the Graph trend series to a non-numeric
    field.
  - Desktop: Grid render mode does not calculate grid cells properly.

### 3.206: 01/30/2010

Bug fixes:

  - Client: More improvements to Palm.

### 3.205: 01/27/2010

Bug fixes:

  - Client: Goto list should automatically update.
  - Client: GPS Marker should use cross-hair style.
  - Client: COM0 is never scanned.
  - Client: Bluetooth Browser is more aggressively disabled.
  - Desktop: Field map generates improperly for Road only view.

### 3.204: 01/20/2010

Bug fixes:

  - Client: More improvements to Palm.
  - Desktop: Timer track sample now generates Goto points.

### 3.203: 01/17/2010

Bug fixes:

  - Client: Overactive timer causes crash on Palm devices.

### 3.202: 01/13/2010

Bug fixes:

  - Client: Crash with long goto point names.
  - Client: Scrollbox scrollbar does not scale properly.
  - Client: Screen state not reset properly after save.

### 3.201: 01/03/2010

Bug fixes:

  - Client: Increase the size of fonts on the GPS screens

New features:

  - Client: Large tabs, large titles, large scroll bars off Application
    Properties

### 3.200: 12/27/2009

Bug fixes:

  - Desktop: Virtual Earth auto-locate no longer works
  - Client: Allow CyberTracker to work with older WinCE devices
  - Client: Upload to local directories should work from desktop
    computer
  - Client: Potential error if GPS fix is ready when pressing Save
  - Client: GPS marker on field map obscures location

New features:

  - Desktop: GPS Simulation
  - Client: Goto feature

### 3.199: 11/21/2009

Bug fixes:

  - Desktop: Fix minor problems with Features sample app

New features:

  - Client: Reset of state on sync

### 3.198: 11/19/2009

Bug fixes:

  - Client: Camera control resolution settings conflict

### 3.197: 11/19/2009

Bug fixes:

  - Desktop: Fix a couple of crashes

New features:

  - Desktop: Convert Measure line into line layer
  - Client: Allow Save targets to be outside the existing path

### 3.196: 11/10/2009

Bug fixes:

  - Desktop: FTP fix from === 3.183 was lost during system migration

### 3.195: 11/05/2009

Bug fixes:

  - Desktop: Check boxes occassionally disappear
  - Desktop: Increase the size of the Map Properties dialog
  - Desktop: Command line use crashes on data export
  - Desktop: Manifest for Windows 7

New features:

  - Desktop: Grid paths option to use active query

### 3.193: 11/02/2009

Bug fixes:

  - Desktop: Efficiency graph: Average start/stop time are not properly
    calculated in some cases

New features:

  - Client: Manual GPS entry

### 3.192: 11/01/2009

Bug fixes:

  - Client: Exporting to a database sometimes has an arbitrary default
    date range.
  - Desktop: Efficiency graph: Distance travelled may change depending
    on the query

New features:

  - Desktop: Bracket with sightings to limit path drawing
  - Desktop: Filter option for query columns
  - Desktop: Improved bulk edit functionality

### 3.191: 10/25/2009

Bug fixes:

  - Client: Entering numbers using the keypad without decimals can
    sometimes fail

New features:

  - Desktop: Create database connection dialog
  - Desktop: Efficiency graph: patrols, speed, average start and stop
    time
  - Desktop: Frequency graph: count per distance
  - Client: Delay GPS Skip button visibility
  - Client: Enter GPS manually

### 3.189: 10/21/2009

Bug fixes:

  - Client: Edge case memory corruption during Field map fixed
  - Desktop: Export of timer tracks doesn't always work
  - Desktop: Importing sightings that are in the deleted state in memory
    will override them
  - Desktop: SQL Server EDB database rules now work properly

New features:

  - Client: Consistent retain state on ElementList, NumberList and
    Keypad
  - Client: Ability to reset state by key

### 3.188: 10/14/2009

Bug fixes:

  - Client: Numerous errors on client caused by overactive memory
    corruption detector

### 3.187: 10/10/2009

Bug fixes:

  - Desktop: Desktop application doesn't upgrade properly

New features:

  - Client: Set desired resolution for camera images
  - Client: Automatic backup to SD card
  - Desktop: Data recovery console

### 3.184: 09/27/2009

Bug fixes:

  - Client: NumberList should support for numbers larger than 500
  - Client: ElementList should display partial items
  - Desktop: Fixes to Grid rendering mode
  - Desktop: Bulk Find and Replace fails if Element occurrence is 0
    (default)

New features:

  - Desktop: Set date range for all queries
  - Desktop: Measure tool on map
  - Desktop: Export CTX from table view
  - Desktop: Properties to customize export of maps as images
  - Desktop: Nautical miles added to Efficiency graph
  - Desktop: Last/Current fiscal year added as relative query date range
  - Desktop: Most editors now have hints below the properties
  - Desktop: Bulk edit has Selection-only option
  - Desktop: Bulk edit has Add for adding meta data

### 3.183: 08/05/2009

Bug fixes:

  - Client: Support for more GMT time zones
  - Desktop: Crashes while adding missing layers
  - Desktop: Cancel after login leaves system in bad state
  - Desktop: FTP transfer doesn't work for some kinds of URL

### 3.182: 07/24/2009

Bug fixes:

  - Client: Potential memory corruption drawing some kinds of triangles
  - Client: SnapTime should resnap when sighting is edited
  - Desktop: Possible to select queries even if they are not active
  - Desktop: Crash on startup accessing web services

New features:

  - Client: R2 Incediary control
  - Client: Element List and Number List can set global variables based
    on selection
  - Desktop: Decimal degree Layers can overlay virtual earth

### 3.181: 06/19/2009

Bug fixes:

  - Desktop: Potential crash when opening a Report
  - Desktop: Icons not updated properly when changed

### 3.180: 05/31/2009

Bug fixes:

  - Desktop: Slow to change queries after a column has been sorted
  - Client: Text result will be cleared if no text is specified on loops

New features:

  - Client: Snap Time action
  - Client: Snap Gps and Snap Last Gps can output to Elements
  - Desktop: Paths can be automatically split if separated by more than
    N minutes

### 3.179: 05/24/2009

Bug fixes:

  - Desktop: Paste Excel filters do not properly handle duplicate names

### 3.178: 05/24/2009

Bug fixes:

  - Desktop: Auto-fix imported data with bad Device Ids
  - Desktop: Fix crash when using advanced query editor
  - Desktop: Path doesn't always update properly

New features:

  - Desktop: Path rendering without requiring Start and Stop Elements

### 3.177: 05/17/2009

Bug fixes:

  - Client: Better handling of device id on the client
  - Desktop: Skip badly formed device ids

New features:

  - Desktop: Auto-detect screen profile for application install

### 3.176: 05/07/2009

Bug fixes:

  - Desktop: Download data from older CyberTracker versions

### 3.175: 04/25/2009

Bug fixes:

  - Desktop: Query grid should retail changes to sort order and column
    width
  - Desktop: Graph view frequency report does not properly decode
    sightings
  - Desktop: Auto-locate faults without firewall bypass
  - Desktop: High-DPI fit and finish
  - Desktop: Compact should use Pack, not just repair
  - Desktop: Remove unneeded sample applications
  - Desktop: Add new sample application: BirdKey
  - Client: Fix memory leak with GPS timer screen

### 3.174: 04/21/2009

Bug fixes:

  - Client: Lock 100 should scale according to the screen profile
  - Client: Use on GPS Skip should be available from the Default Field
    Map

New features:

  - Client: GPS Timer screen is now more customizable
  - Desktop: Virtual Earth now auto-locates based on IP address

### 3.173: 04/16/2009

Bug fixes:

  - Desktop: Crash when temp directory is on a different drive to
    CyberTracker system directory

New features:

  - Client: Element Panel control

### 3.172: 04/14/2009

Bug fixes:

  - Desktop: Crash while pasting filters on account of new UI components
  - Desktop: Modify paste feature to allow isolation of same-named
    category elements

### 3.171: 04/12/2009

Bug fixes:

  - Desktop: Change 'Moving Map' to 'Field Map' for improved clarity
  - Client: Skip GPS to Moving Map sometimes crashes

New features:

  - Desktop: Global Field map which applies to all applications
  - Desktop: Field map creation from existing maps
  - Desktop: Ability to sign CTX files with author and owner information
  - Desktop: Remove ECW Creator
  - Client: Center Text feature on Element List
  - Client: Rework zoom image so entire image fits on screen at once
  - Client: Lock 100 feature prevents zooming in below 100 %

### 3.170: 03/17/2009

Bug fixes:

  - Client: Fix broken zoom function on moving map
  - Client: Zoom in and zoom out not functioning properly
  - Client: Decrease sleep on background thread to increase acquisition
    time

### 3.169: 03/15/2009

Bug fixes:

  - Desktop: Map "Copy to Clipboard" doesn't always fill in Virtual
    Earth correctly
  - Desktop: Map Export to JPG/BMP doesn't export Virtual Earth
    correctly
  - Desktop: Add more descriptive text when database version is wrong
  - Desktop: New applications have "Test time on startup" unselected by
    default
  - Desktop: Exporting map should not show legend if only one query is
    active
  - Desktop: Re-add "Open Sample" feature
  - Client: Fix broken zoom function on moving map
  - Client: Moving map should be able to handle arbitrary zoom

### 3.168: 02/04/2009

Bug fixes:

  - Desktop: Crash when placing a Send Data control on the screen
  - Desktop: Layout mode button doesn't stay down
  - Desktop: Static element have duplicate Inclination
  - Desktop: Re-add X86 PPC build

### 3.167: 02/03/2009

Bug fixes:

  - Desktop: Overactive error message regarding being not properly
    installed

### 3.166: 02/02/2009

Bug fixes:

  - Desktop: CyberTracker should not change the current working
    directory (for command-line usage reasons)
  - Desktop: Change Sequences to Applications
  - Desktop: Ensure CyberTracker is properly registered if ActiveSync
    was installed after CyberTracker
  - Desktop: Only show Import dialog if some of the properties are set
  - Desktop: Remove Player and Studio concept
  - Desktop: Move current alias to Application Properties dialog
  - Desktop: Fix crash when opening reports
  - Desktop: Fix crash when changing colors on maps
  - Desktop: Split Application properties over multiple tabs

10.Desktop: Add icons to several menu options

  - Desktop: Remove "Set Media" feature from Element mode
  - Desktop: Change database directory from "My CyberTracker Databases"
    to "CyberTracker"
  - Desktop: Change install directory to "CyberTracker3"
  - Desktop: Upgrade to latest version of UI components

New features:

  - Desktop: Allows more control over available features when not logged
    in
  - Desktop: Ability to load and save CTX files
  - Desktop: Ability to send CTX files via email

### 3.165: 12/14/2008

Bug fixes:

  - Desktop: Map projections should accept latitudes and longitudes in
    degrees, not radians

### 3.163: 12/09/2008

Bug fixes:

  - Client: GPS should not be on when not in use on WM5+ devices
  - Client: GPS thread should not be executed at below normal priority
  - Client: Date format should come from device preferences

New features:

  - Client: "Disable editing" to reduce errors

### 3.162: 12/07/2008

Bug fixes:

  - Client: Fix fault on older Palm devices

### 3.161: 12/07/2008

Bug fixes:

  - Client: Time should be in 24 hour format
  - Desktop: Fix crash with unsupported SID files
  - Desktop: Fix race condition with upload directory and upload
    sequence locks

New features:

  - Client: New control "System" data, e.g. time, battery
  - Client: Navigator can have the Back button hidden via the "Show
    back" property
  - Client: Upload data control is now iconic

### 3.160: 11/30/2008

Bug fixes:

  - Client: Ensure GPS time always in sync
  - Client: Kiosk mode not enabled after a reset

New features:

  - Client: Right to left property for Element Lists and Memos

### 3.159: 11/25/2008

Bug fixes:

  - Client: Re-calibrate GPS for TDS Nomads, so date/time/heading/speed
    information is sent

### 3.158: 11/23/2008

Bug fixes:

  - Client: Wrong time zone set

### 3.157: 11/23/2008

Bug fixes:

  - Client: Force Nomad to use NMEA, so it can get date and time
  - Client: Minor cosmetic improvements for HighDPI
  - Desktop: Add Geocentric datum for Israel
  - Desktop: Map co-ordinates sometimes 100+ meters wrong for UTM

### 3.156: 11/22/2008

Bug fixes:

  - Client: Keypad should not store passwords as state: leaving the
    screen always clears
  - Client: Native Windows Mobile GPS not always selected when available

New features:

  - Client: Element Formula control now has Hidden property
  - Client: Element Formula control has the ability to add new screens
  - Desktop: Bulk edit of sightings

### 3.155: 11/15/2008

Bug fixes:

  - Desktop: Fix crashes associates with making certain properties lock
    visible, e.g. Hide links, Notebook Pages
  - Desktop: Multiple copies of the same sequence on device
  - Desktop: Robustness improvements to importing mechanism
  - Desktop: Fix crash related to media not prepared

New features:

  - Client: Kiosk mode
  - Client: Add password functionality to Element Keypad control
  - Client: Add maximum length to text fields
  - Desktop: Export from full database query via command line
  - Desktop: Add datum EUROPEAN 1950, Portugal & Spain

### 3.154: 11/02/2008

Bug fixes:

  - Desktop: Update client if transfer settings have changed
  - Desktop: File-share transfers should support username and password

New features:

  - Client: HTTP and HTTPS uploads

### 3.153: 10/27/2008

Bug fixes:

  - Desktop: Convert transfer into URL style to support more protocols
  - Desktop: Create upload CAB files atomically
  - Desktop: Ensure CABs are well formed before download
  - Desktop: Move all Transfer features under the Transfer tab
  - Desktop: Change "Lock" to "Layout"
  - Desktop: Change command line FTP references to URL to support more
    protocols
  - Desktop: Prevent duplicate sightings when "Clear on Send" is
    disabled
  - Desktop: Fix crash when failing to update the registry during sync
  - Desktop: Fix crash during reports caused by a synchronization issue

New features:

  - Client: Option to bypass "Time wrong" errors
  - Desktop: Refresh feature for Report mode (F5)
  - Desktop: Download from file share

### 3.152: 10/23/2008

Bug fixes:

  - Desktop: MySQL export should ensure floating point numbers have
    locale invariant form
  - Desktop: Fix crashes caused by editors being out of sync with
    underlying object in rare cases

New features:

  - Client: Sync PDA time with GPS time
  - Client: Speed, heading, UTC date and time are displayed on the GPS
    screen

### 3.151: 10/14/2008

Bug fixes:

  - Client: Extend timeout for GPS detection on PalmOS
  - Client: GPS viewer screen has title bar below spacer

New features:

  - Client: Auto-send every X minutes

### 3.150: 10/05/2008

Bug fixes:

  - Desktop: Date conversion doesn't always work

New features:

  - Desktop: Crash recovery

### 3.149: 09/28/2008

Bug fixes:

  - Desktop: Always store and export floating point numbers using . as
    separator
  - Desktop: Export to shape file of Virtual Earth should always use
    WGS84 datum
  - Client: New timer mechanism

### 3.148: 09/02/2008

Bug fixes:

  - Desktop: Connecting to MySQL on Linux database test
  - Desktop: Improve performance of Windows Mobile sequence upload

### 3.147: 08/28/2008

Bug fixes:

  - Desktop: Connecting to MySQL on Linux database test

### 3.146: 08/23/2008

Bug fixes:

  - Desktop: More descriptive error message on database connection
    failures
  - Client: Input button not being hidden correctly after editing
  - Client: Display errors on Text and Keypad screens when no Result
    Element is specified

### 3.145: 08/20/2008

Bug fixes:

  - Client: Fine tuning for range finder control
  - Client: Reduce retry count on serial port reads

### 3.144: 08/18/2008

Bug fixes:

  - Desktop: === 3.143 may not have been a valid build
  - Client: Re-added WM5 GPS support after testing on Travel Companion
  - Client: Support for Trupulse 360 RangeFinder
  - Client: Device threads should be set to below normal priority

### 3.143: 08/14/2008

Bug fixes:

  - Desktop: Media2 table was sometimes being referenced as MEDIA2
  - Client: Re-added WM5 GPS support after testing on Travel Companion
  - Client: Partial support for Trupulse 360 RangeFinder

### 3.142: 07/29/2008

Bug fixes:

  - Desktop: Failed to move to Outgoing folder (CT11)
  - Desktop: Download should be to specified database, not Staging

### 3.141: 07/27/2008

Bug fixes:

  - Desktop: Crash when changing columns on Element Editor
  - Desktop: Crash when pasting filters
  - Desktop: FTP upload and download support not working when database
    locked

### 3.140: 07/23/2008

Bug fixes:

  - Desktop: Working on the command line mechanism

### 3.139: 07/16/2008

Bug fixes:

  - Desktop: Upload on application start should be asynchronous

### 3.138: 07/16/2008

New features:

  - Desktop: Upload sightings to FTP site on Sync
  - Client: Turn of send via FTP

### 3.137: 07/14/2008

New features:

  - Desktop: Ability to control CyberTracker from the command line
  - Desktop: Download sightings from FTP site

Bug fixes:

  - Desktop: FTP settings should be on Database Properties dialog
  - Desktop: Passwords should be represented with the password character
  - Desktop: Crash when closing CyberTracker
  - Desktop: Don't scan all databases on startup
  - Client: Send data should only be available if configured

### 3.136: 07/02/2008

Bug fixes:

  - Desktop: Assertion error after modifying media
  - Desktop: Media errors when connecting to external databases
  - Client: Do not delete outgoing data during uninstall
  - Client: GPRS support for send data

### 3.135: 06/30/2008

New features:

  - Desktop: Connect to MySQL via external database definition files

### 3.134: 06/22/2008

Bug fixes:

  - Desktop: XML parser leaks small amounts of memory

New features:

  - Client: Upload to FTP (BETA)

### 3.133: 06/13/2008

Bug fixes:

  - Desktop: Download data device broken on Windows Mobile
  - Desktop: Feature files specified on command line not respected

### 3.132: 06/12/2008

Bug fixes:

  - Install: Install was still broken on non Palm systems

### 3.131: 06/11/2008

Bug fixes:

  - Install: Install was broken

### 3.130: 06/10/2008

Bug fixes:

  - Desktop: Crash after clearing rows in some grid editors
  - Desktop: Cannot copy to clipboard from query table
  - Desktop: Error 103 when synchronizing a Palm on Vista
  - Desktop: File association does not work if filename has a space
  - Desktop: VirtualEarth race condition regarding internet access
  - Desktop: XML database fields should specify encoding and handle it
    correctly

New features:

  - Client: Element list retain only scroll state
  - Desktop: Samples moved under databases
  - Desktop: Icons and samples will be a separate download
  - Desktop: Player and Studio versions
  - Desktop: High resolution icons
  - Desktop: More efficient packaging: fewer files
  - Desktop: Studio and regular versions instead of Professional,
    Standard and Viewer
  - Desktop: Improved XML handling to remove out-of-memory conditions
  - Desktop: Improved media handling for performance

10.Desktop: Media for sightings is now housed alongside regular media

  - Desktop: Sighting table can have XmlData column for interop with
    other systems
  - Desktop: Synchronize is now called Install

### 3.129: 05/05/2008

Bug fixes:

  - Desktop: Crash when pasting filters
  - Desktop: Remove date restriction on Virtual Earth implementation

### 3.128: 04/13/2008

Bug fixes:

  - Desktop: Crash when adding map image after using Virtual Earth
  - Desktop: Crash when exporting elements to invalid location

New features:

  - Desktop: Trend graphs
  - Desktop: Copy to clipboard for views

### 3.125: 03/26/2008

Bug fixes:

  - Desktop: Crash when adding columns very quickly

### 3.124 (BETA): 03/21/2008

Bug fixes:

  - Desktop: Disable delete on property editors
  - Desktop: Occasional crash when exit while disconnecting Treeview
  - Desktop: Delete key on a color editor causes crash
  - Desktop: Loading database uses too much memory
  - Client: Disable WM5 GPS code again

### 3.123 (BETA): 03/02/2008

Bug fixes:

  - Client: Map control produces incorrect readings on Skip
  - Client: Remove EnsureResultOnSave concept
  - Client: Use RangeFinder for altitude on Configure GPS
  - Client: Enable WM5 GPS code again

### 3.122 (BETA): 02/27/2008

Bug fixes:

  - Desktop: Elements not properly updated when deleting from Elements
    mode
  - Desktop: Crash when editing Photos Element of Camera

### 3.121 (BETA): 02/25/2008

Bug fixes:

  - Desktop: Crash when pasting Actions
  - Desktop: Data loss: special characters are lost from text
  - Desktop: Tree doesn't retain scroll state after delete
  - Desktop: Tree doesn't retain correct selection after drag/drop
  - Desktop: Installer should not allow launch after install on Vista

### 3.120 (BETA): 02/16/2008

Bug fixes:

  - Client: Scrollbar sometimes doesn't start at the top
  - Desktop: Filter screens are slow
  - Desktop: Loading large databases is slow
  - Desktop: Reduce memory foot of undo buffer
  - Desktop: Generalize 'Paste From Excel' feature
  - Desktop: Memory leak in Virtual Earth

### 3.119 (BETA): 02/11/2008

Bug fixes:

  - Client: Fix hang when using GPS screen

### 3.118 (BETA): 02/10/2008

Bug fixes:

  - Client: Rename Element to Result Element where appropriate
  - Client: Moving map control should be able to retain state
  - Client: Temporarily disable Windows Mobile 5 GPS code
  - Desktop: Crash when re-ordering tree items with keyboard and mouse
    together
  - Desktop: Repaint issues when Element has a . in the name
  - Desktop: Add button to allow removal of Sound once specified

### 3.117 (BETA): 01/29/2008

Bug fixes:

  - Client: Follow icon does not appear on moving map on PocketPC

### 3.116 (BETA): 01/25/2008

Bug fixes:

  - Desktop: TMP files are not properly cleaned up from Databases folder
  - Desktop: Crash when editing sightings using Edit Sighting dialog
  - Desktop: Grid rendering default values tweaked

### 3.115 (BETA): 01/13/2008

Bug fixes:

  - Client: Default setting is not to block radio next
  - Desktop: Next screen sometimes fails after deleting the old last
    screen
  - Desktop: Clean Paths should reset the waypoint source

### 3.114 (BETA): 01/13/2008

Bug fixes:

  - Desktop: Reduce the chance of failure during database compaction on
    save
  - Desktop: Fail safe to ensure download log messages are written, even
    if a lock exists on the file
  - Desktop: Pressing cancel on close on exit dialog after redirection
    allows accidental no-save exit
  - Desktop: Relocate map properties to be next to the map view for
    easier customization
  - Desktop: Improvements to Grid rendering
  - Desktop: Point and path renderer colors should be the same

### 3.113 (BETA): 01/08/2008

Bug fixes:

  - Client: Fall through to serial GPS if Windows Mobile 5 GPS is not
    hooked up
  - Desktop: Property editor clears when changing image co-ordinates on
    Map View Properties
  - Desktop: Crash when saving and reloading from virtualized locations
    on Vista
  - Desktop: Manifest all CyberTracker components to understand Vista
    UAC
  - Desktop: Improve error messages when attempting to Save or Sync
    samples
  - Desktop: Map View Grid rendering improvements to work more correctly

### 3.112 (BETA): 01/06/2008

Bug fixes:

  - Desktop: Fix crash when editing a number and clicking Lock during
    sequence editing
  - Desktop: Right cliDesktop: Right click context menu should not
    deselect list items
  - Desktop: Fix crash when adding a graph view: introduced in === 3.111
  - Desktop: Improve performance of Map View Properties dialog
  - Desktop: Map View Desktop: Map View Properties dialog incorrectly
    resets the bounds even if no change occurs
  - Desktop: Map View Grid rendering improvements to work more correctly

### 3.111 (BETA): 01/01/2008

Bug fixes:

  - Client: Scale GPS bars to max SNR of 55 instead of 100
  - Client: Text color not an exposed property for navigator buttons
  - Client: "Element Aggregate" should be renamed "Element Formula"
  - Client: Right click menu should appear on mouse-up not mouse-down
  - Client: Drag and drop should not focus tree nodes
  - Desktop: System folder should not be hidden
  - Desktop: Time column converts to date for advanced queries
  - Desktop: Editing in inspector not always reflected in table
  - Desktop: Extend Virtual Earth expiration date to April 2008

New features:

  - Client: Auto-next screen if no next screen available
  - Client: Windows Mobile 5 and above native GPS support
  - Client: New icons for Save 1 and Save 2
  - Client: "Radio element" is stored as a reference to an Element, so
    it works in filters
  - Client: Check lists store results as a check box
  - Desktop: Client context menu for deleting and cut, copy and paste of
    controls
  - Desktop: New sequence wizard should allow creating a copy of the
    existing one
  - Desktop: Improved copy and paste for controls, elements and screens

### 3.110 (BETA): 11/22/2007

Bug fixes:

  - Client: Breaking change: Always run Next rules before saving
  - Client: Invalid GPS coordinates when using SnapGPS on the Save
    screen
  - Desktop: Crash after closing Virtual Earth Map
  - Desktop: Occasional crash when unable to open database

### 3.109 (BETA): 11/17/2007

Bug fixes:

  - Client: Increased the minimum scrollbar thumb slightly to improve
    appearance
  - Client: Fixed an Assert failure when navigating between screens with
    Auto next turned on
  - Client: Changed "Time out of sync" to "Time is wrong"
  - Desktop: Reworked the crash exception mechanism to provide more
    information on failures
  - Desktop: Fixed a synchronization bug in the Virtual Earth
    multi-threading code
  - Desktop: Changed the minimum value from 0 to -999999999 so that
    negative numbers can be used
  - Desktop: Exporting shape files from Virtual Earth should not export
    as Virtual Earth projection
  - Desktop: Extended Virtual Earth feature expiration date to
    12/31/2007 ===

### 3.108 (BETA): 10/31/2007

Bug fixes:

  - Desktop: Fixed several newly reported crashes generated by the
    updated tools
  - Desktop: Re-added ConvertCTZ to the full professional version

### 3.107 (BETA): 10/30/2007

Bug fixes:

  - Desktop: Failure to load client.dll on many systems

### 3.106 (BETA): 10/29/2007

Bug fixes:

  - Desktop: Rebuilt on reports of failure to load sequences

### 3.105 (BETA): 10/29/2007

Bug fixes:

  - Desktop: Hotsync fails to start

### 3.104 (BETA): 10/29/2007

Bug fixes:

  - Client: Improve support for negative numbers on keypad
  - Client: Improve support for negative numbers on number list

New features:

  - Desktop: Virtual Earth on map views
  - Client: Added new number list style

### 3.103: 09/29/2007

Bug fixes:

  - Desktop: Map rebuilds when closing: performance issue
  - Desktop: Accuracy threshold doesn't filter paths correctly
  - Client: Number keypad doesn't handle decimals properly

### 3.102: 09/26/2007

Bug fixes:

  - Desktop: Crash with some map images: Assert failure in mapping
    software
  - Client: Formulas always come out negative

### 3.101: 09/22/2007

Bug fixes:

  - Desktop: Crash while editing categories on Element Filter
  - Desktop: Map layers do not always hide/show correctly

### 3.100: 09/20/2007

Bug fixes:

  - Desktop: Crash while handling deferred map resize message
  - Desktop: Date ranges don't work properly for Last 1,2,3 days
  - Desktop: Can't export shape files if column with multiple NULL
    fields is active
  - Desktop: Performance problems with huge timer track datasets and
    multiple queries

### 3.099: 09/08/2007

Bug fixes:

  - Client: Fix title bar to pick up screen title correctly and work in
    High DPI
  - Client: Keypad buttons disappear when scale is too small
  - Desktop: Deleted Elements visible in Element find mode

New features:

  - Client: Add negative number support to keypad
  - Client: Add one-line only property to text entry
  - Client: Add required property to text entry
  - Desktop: Point and Path renderers can customize timer point size and
    line width

### 3.098: 08/26/2007

Bug fixes:

  - Client: Fix crash when editing notebook pages
  - Desktop: Map zoom changes are incorrectly added to the undo buffer
    when resizing the map window
  - Desktop: Map query cursors are not propertly cleared when changing
    queries

New features:

  - Desktop: Improve query date range types
  - Desktop: Map background queries can have transparency
  - Desktop: Queries from non-active queries are now selectable
  - Desktop: Point rendering: timer tracks are visible for all queries
  - Desktop: Path rendering: timer tracks are visible for all queries

### 3.097: 08/03/2007

Bug fixes:

  - Desktop: Fix Windows 2000 bug when creating image resources for the
    client
  - Desktop: Crash when viewing sightings that have pictures associated
    with them
  - Desktop: Feature file editor does not show check boxes when themes
    not enabled

New features:

  - Desktop: Added label support for shape files on Map View

### 3.092: 07/14/2007

Bug fixes:

  - Desktop: Map disappears when co-ordinates are inverted
  - Desktop: Failure to sync if client data file has missing header

### 3.091: 07/03/2007

Bug fixes:

  - Client: Fix broken GPS timer on devices with built-in GPS support

### 3.090: 06/22/2007

Bug fixes:

  - Desktop: Allow less than \* 0 for GPS accuracy settings
  - Desktop: Ensure Uncategorized Elements are properly visible after
    merges
  - Client: Ensure Soft Input Panel (SIP) is not visible on Windows
    Mobile 5 devices
  - Client: Ensure database header is validated for sighting database
    always available

### 3.089: 03/11/2007

Bug fixes:

  - Client: Buffer overflow on Palm when working with strings

### 3.088: 03/04/2007

Bug fixes:

  - Client: 2 minute and longer timer automatically turns off after 12
    minutes if unattended
  - Client: Undownloaded sightings can be incorrectly detected

### 3.087: 02/25/2007

Bug fixes:

  - Client: HighDPI screens have scroll buttons that are scaled
    incorrectly.

New features:

  - Client: Added support for global variables.

### 3.086: 02/11/2007

Bug fixes:

  - Client: Don't add to the track database if the track timer is off or
    we are using a high resolution timer
  - Client: Don't delete sightings if the state file is out of sync with
    the desktop

New features:

  - Client: Added date support to the formula system for the Element
    Aggregate control

### 3.085: 01/01/2007

Bug fixes:

  - Desktop: Fixed memory corruption issue when Syncing to Palm devices

### 3.084: 12/31/2006

Bug fixes:

  - Desktop: Improved performance of Sequence Designer for screens with
    lots of controls
  - Desktop: Removed "Plain Text" export, because it is not used often
    and has bugs
  - Desktop: Colors in sequence could appear differently on Client
  - Client: Element Calculator Control functions are now case
    insensitive
  - Client: Element Calculator Control now has 26 variables instead of 3
  - Client: Element List: number keypad now has Min and Max bounds
  - Client: Scroll box: scroll bar occasionally becomes invisble

### 3.083: 12/21/2006

Bug fixes:

  - Desktop: Fixed bug introduced in === 3.082 causing all features to
    be enabled on Standard and Viewer
  - Desktop: Fixed auto-select of the first screen when changing
    sequences
  - Desktop: Fixed Wildlife with data sample - text sequence links
    broken

New features:

  - Client: Element Calculator control now supports full expressing
    parsing

### 3.082: 12/17/2006

Bug fixes:

  - Desktop: Fixed Crash during Element Editing in Sequence mode
  - Desktop: Fixed menu option inconsistency after import with password
    changes
  - Desktop: Remove MrSID support files for Min build

New features:

  - Client: Element Calculator control for performing mathematical
    calculations on Element values
  - Client: Element List support for a keypad popup when an Element is
    selected. This works with the Number List style and the "Use keypad
    for numbers property".
  - Client: Element List and Element Keypad support single denominator
    fractions.

### 3.081: 12/04/2006

Bug fixes:

  - Desktop: Sighting and Waypoint query don't work on non-US date
    formats (broken since === 3.079)
  - Desktop: auto-detect help files and run locally if present
  - Client: Zero should be allowed for number keypad screens

New features:

  - Desktop: Minimum version for smaller download sizes

### 3.080: 11/24/2006

Bug fixes:

  - Desktop: Synchronization should fail more cleanly if PocketPC not
    connected
  - Desktop: Fix crash when using Undo and Tree is being edited
  - Desktop: XML format should be more generic
  - Desktop: Edit Sighting dialog should allow negative values for
    latitude and longitude
  - Desktop: Should be able to edit Latitude and Longitude in the grid
  - Desktop: Change toolbar buttons to fit into 800x600 resolution
  - Desktop: Improvements to Samples

New features:

  - Client: SnapLastGPS Action which takes the last valid GPS reading
    and attaches it to a sighting

### 3.078: 11/12/2006

Bug fixes:

  - Desktop: Improve synchronization reliability

New features:

  - Desktop: Password protection system so users without a password
    cannot edit sequences/elements
  - Desktop: Map: Cleanup tracks which deletes unused timer points
  - Desktop: Import Data Only: Ability to import multiple CTX files at
    once

### 3.077: 10/28/2006

Bug fixes:

  - Client: Expose scroll bar width as a changeable property on controls
  - Client: Correct Navigator Jump functionality to work as expected
    with Radio lists
  - Desktop: Expose "Outlier Speed" - should apply to all map renderers
  - Desktop: Should only attempt to install PocketPC client when
    connection has been correctly established

New features:

  - Desktop: "Accuracy threshold" for path generation and efficiency
    reports

### 3.076: 10/26/2006

Bug fixes:

  - Desktop: Allow PocketPC sync to crash on hard errors instead of
    failing silently
  - Client: Improvements to Navigator control
  - Client: Sighting editing was broken

New features:

  - Client: Navigator Button Controls which can have images assigned to
    them

### 3.075: 10/17/2006

Bug fixes:

  - Desktop: Changing point color should change track color
  - Desktop: Performance improvements to sightings and tracks
  - Desktop: Improve semi-colon delimited list support
  - Client: Element list sometimes leaves play and stop buttons visible

### 3.074: 10/02/2006

Bug fixes:

  - Desktop: Using Cancel while changing map image crashes
  - Desktop: Screens without assigned images prevent sync
  - Desktop: Improve path detection when 2 subsequent sightings have the
    "Start Element"
  - Client: PocketPC cannot press Enter for notes screens
  - Client: Element Keypad doesn't support decimals properly

New features:

  - Desktop: Semi-colon delimit selections made from check lists

### 3.073: 08/18/2006

Bug fixes:

  - Desktop: GPS acquisition doesn't complete - triangle never shows
  - Client: Restrict time that triangle shows

New features:

  - Desktop: Snap GPS Action now has "Auto connect" property
  - Desktop: RangeFinder Style property can be Range only

### 3.072: 08/16/2006

Bug fixes:

  - Desktop: Importing external screen templates doesn't update treeview
    correctly
  - Desktop: Added simple screen templates
  - Desktop: Auto expand New Screen templates treeview
  - Desktop: Help files should not reference "Major" and "Minor" targets

New features: None.

### 3.071 BETA: 08/14/2006

Bug fixes:

  - Desktop: Simple path rendering used when no Join Elements specified
  - Desktop: Crash when closing map view during slow calculations

New features:

  - Desktop: Efficiency graph now uses the path building system for
    calculations and includes outlier detection

### 3.070 BETA: 08/12/2006

Bug fixes:

  - Desktop: Path doesn't correctly join when separated by waypoints

New features:

  - Client: ElementList has a "Sorted" property which sorts the list by
    caption: slow on the desktop, but fast on the device
  - Desktop: ElementList "Element" editor has a "Sort" button which
    sorts the list alphabetically

### 3.069 BETA: 07/25/2006

Bug fixes:

  - Client: Keypad calculator control should have buttons in same order
    as real calculator
  - Desktop map: active query is now brought to front or render order
  - Desktop map: Grid rendering now always renders grid in the same
    location regardless of zoom
  - Desktop map: Grid export should export data unscaled
  - Desktop map: Path calculations incorrectly breaks path if endpoints
    are more than 1 hour apart

New features:

  - ElementList has a "Hide links" property which significantly speeds
    up the UI when dealing with large lists of Elements when none of
    them need to point to a specific screen.
  - Map has a Refresh button which allows you to update it when the
    extents change for Grid mode
  - Grid rendering now has "Low effort threshold" property
  - Grid rendering now has "Outlier detection speed (km/h)" property

### 3.068 BETA: 07/24/2006

Bug fixes:

  - Desktop: Viewer toolbar is now invisible (it only had one button
    which was wasting space)
  - Desktop: map points dissappear when zoomed in too much with huge map
    extents
  - Desktop: Creating controls in "Lock" mode should work everywhere on
    design surface
  - Desktop: Import all staged sightings on startup, not just on sync
  - Desktop: Crash while adding columns
  - Client: MobileMapper CE GPS does not detect properly
  - Client: Changes to support Thales MobileMapper (WinCE) as well as
    PocketPC
  - Client: Windows Start button disappears after using a sequence
  - Client: Does not uninstall on WinCE
  - Client: Improve the handling of "Time out of sync" errors between
    handheld and PC
  - Client: Timer list should include 1 second timer (and remove 4
    minute timer) interval
  - Client: Handle old sequences left on the device properly
  - Client: Changes to GPS timer are overridden by sequence properties
  - Client: fast/slow GPS track timer threshold should be 1 minute, not
    30 seconds
  - Client: RangeFinder state should persist between exit/restart
  - Client: GPS and RangeFinder should never block other UI
  - Client: Improved screen load performance on slower systems
  - Client: Titlebar options button should be more easily clickable
  - Client: Added support for LA1KC RangeFinder message

New features:

  - Desktop: support for Index of Abundance / Effort of Patrol / Cell
    count
  - Client: Panel has a "Use screen name" property which causes it to
    take the name of the current screen as its caption. This means that
    creating new screens is faster because you only have to type the
    name of the screen and the title will match.
  - Client: SnapGPS Action now has a "Required" property which allows
    you to make it optional, i.e. it will take a GPS reading if
    available.
  - Desktop: Help menu now points to FAQ and Tutorial Movies.
  - Desktop: Controls are now hosted in an auto-hiding Toolbox, instead
    of just being in a simple vertical toolbar. This makes them easier
    to see and use, because when visible you can see the full control
    name. They are also categorized into "Static controls", "Data
    controls" and "Actions".
  - Desktop: Path rendering is now available off View Properties for the
    Map. Paths allow you to control how timer tracks are used to join
    observations.
  - Client: New Action: Configure Save Targets: this replicates the
    functionality of the "Ok destination" from version 2
  - Client: Lists have a "Radio Element" property which allows you to
    have the text of a radio list selection assigned to an Element. This
    is useful for cases when you don't want to have to duplicate long
    lists of Elements to capture different fields that are identical
    except for context, e.g. Observer 1 Name and Observer 2 Name.
  - Desktop: Elements mode has a new menu option called "Export Elements
    to Table" which allows you to save the contents of the grid to an
    Excel file. This is useful for copying Elements between different
    sequences as well as being a general way to export Elements out of
    CyberTracker.
  - Desktop: Export Data-only - available off the file menu, allows
    export of data only files which are much smaller, but don't contain
    sequences
  - Desktop: Screen Elements edit has "Move First" and "Move Last"
    buttons to help with re-ordering of large lists of Elements.
  - PocketPC: Multiple sequence support. The PocketPC front-end has been
    rewritten to enable multiple sequences to be loaded onto a device at
    the same time.
  - PocketPC: Task bar visibility. The new front end has an option to
    show/hide the taskbar for a sequence.
  - Desktop: Screen profiles are now a global setting which affect all
    sequences. Unfortunately this change means that if you created any
    of your own profiles in the past, you will need to recreate them.
    "Configure Profiles" is now available off the "Tools" menu.
  - Desktop: Screen snapshot to clipboard. There is a new option in the
    Sequence writer to take a snapshot of the active screen and copy it
    to the Windows clipboard. This makes it easier for document writers
    to cut-and-paste images into their applications.
  - Code preparation for the SDK: the client side (on the PDA) will be
    made OpenSource with the MPL. The way it is structured, this will
    allow third party developers to create custom controls and actions
    that tweak the behavior of the client. We expect this to be released
    in the next month.

Design change:

  - Desktop: When viewing data on the map, all queries are
    simultaneously visible. This is now optional and off by default,
    i.e. by default, the map only shows the active query. You can get
    the old behavior by checking the "Show all queries at once" property
    in the new Render tab of the Map's View Properties.
  - Desktop: Shape file Export is now available when exporting from the
    Map. Previously, it was available from the Table.

### 3.058 BETA: 06/24/2006

Bug fixes:

  - Fixed crash when re-ordering columns with active query set
  - Fixed render order for shape files when map image is set

### 3.057 BETA: 06/20/2006

Bug fixes:

  - Double values not displayed properly in Sighting history
  - Text from text editors should have leading and trailing spaces
    removed
  - Opening COM0 on some PDAs causes a hang, removed this from detection
    code
  - Added 57600 as a baudrate for the GPS auto-detect
  - Error in sequence when loops within loops are used
  - Desktop: Color selector should retain custom colors
  - Desktop: Auto-next sometimes confuses screen editor

New features:

  - Atlanta Laser Range Finder support
  - 3 new controls: "Range Finder" (for status), "Element Range Finder"
    (for data) and an action "Configure Range Finder" for support of the
    Atlanta serial Range Finders.
  - Static Elements for range, roll, inclination and bearing.
  - "Alignment" property added to Panel and Memo controls Text can now
    be aligned left, center or right in Panel and memo controls.
  - "Require non-zero" property added to Element Keypad. This will
    prevent a "Next" if the value has not been set to something other
    than zero.
  - "Element Memo" now accepts Name as an attribute
  - "Ensure result on save" property added to Navigator. This prevents
    save if the result on the current screen is required, i.e. will
    prevent save until the current screen contains valid data.
  - "Retain state" for Element Number List The Element Number List now
    supports "Retain state" in the same way as Element Lists do.

### 3.056 BETA: 06/06/2006

Bug fixes:

  - Crash when double-clicking on elements to create new columns
    (introduced by perf improvements in === 3.053)
  - Crash caused by race condition when synchronizing PocketPC at the
    same time as an ActiveSync was happening

New features:

  - Sound support for MP3 files in addition to WAV files on PocketPC.
    Sound files tend to be very large - much bigger than images. MP3 is
    still one of the better compression technologies around and we now
    support this format on both the desktop and PocketPC. Sound is not
    supported on Palm.
  - New view type: Graphs. We have added a new view type for graphs. So
    far we have Frequency and Efficiency tabs. If you used them in
    version 2 and were missing them, they're back. They also support
    exporting to all the usual formats (XML, XLS, TXT, HTM). Note, we
    don't support printing since Excel does such a good job of this
    already.

### 3.053 BETA: 05/19/2006

Bug fixes:

  - Sound should stop when leaving a screen on which sound was playing
  - Left-most navigator buttons should shunt left when possible
  - Palm: when using large images with Elements, element names sometimes
    disappeared
  - Desktop: Performance problems when dealing with lists with a large
    number of Elements

Design change: Mid-sequence loops are now handled Whenever a loop is
detected in a sequence, it is now automatically removed and attributes
that are set within the loop are preserved. For example, if a sequence
goes:

```
A -> X -> Y -> Z -> X
```
then CyberTracker will preserve any attributes set in screens Y and Z and the final path will be:

```
A -> X (with X being the active screen)
```
In the past, this only worked from the start screen and only the last attributes were preserved. We are trying out this behavior to see if it is useful.

New features:

  - Home button. The Navigator control can now also show a "Home"
    button. The icon looks like a house. Clicking on this button is the
    same as pressing the back button until that screen is reached. See
    the "Show home" property. You can also enable the "Home Screen"
    target by checking it in "Lock Properties".
  - Sound support on Radio lists You can enable a "play" button on radio
    lists by checking the "Show radio sound" box on the list control.
    When enabled, a play button will appear next to the current selected
    item. This only works for radio lists and requires that the
    Element's sound property be set. See also: "Show radio sound stop".
  - Auto next for radio lists. You can enable "Auto next" for radio
    lists by checking the "Auto radio next" property of the list
    control. This only works if the list is a radio list, check and
    number lists work the same as before.

### 3.052 BETA: 05/08/2006

Bug fixes:

  - Failure to download Elements when synchronizing sequences with no
    elements
  - Memory leak with screen names
  - Normal shutdown sequence not always followed on client

New features:

  - Wave sound support on PocketPC To access this feature you will need
    the Professional version. Select "Lock" in the Sequence editor and
    then drop either the "Sound" or "Element Sound" control onto a
    screen. Note, we currently only support PocketPC and Wave sound
    files.
  - Palm GPS track log sometimes stops. If the Palm application is
    exited for any reason other than a normal close (via the titlebar on
    the Options dialog) AND a track timer is active, then a 60 second
    alarm will be set to restart CyberTracker and continue the track.
    This is to handle cases where track logs are interrupted by other
    applications.

### 3.050 BETA: 05/06/2006

Bug fixes:

  - SE08 error when working with reports
  - Report dates not preserved when using different date formats
  - Sample databases had uninitialized links which caused the skip
    button to occasionally show in design mode.

New features:

Force Title Bar. To access this feature, select "Sequence Properties"
from the desktop Sequence editor and then check the "Force title bar"
checkbox. This makes CyberTracker a better Windows Mobile citizen by
always having a titlebar with an exit button on it. Note, if your screen
has a panel at the top, then it will replace this panel and use its
text, otherwise it will use the screen name.

### 3.049 BETA: 04/27/2006

Bug fixes:

  - Crash on DownloadCE when device cannot get a device id
  - Crash when using a Title Bar control with a less than 5 character
    title on PocketPC
  - GPS Position lost after editing a sighting

New features:

Add User Name. To access this feature, run the Professional version and
do the following on the first screen:

  - Click "Lock" on the Toolbar
  - Select the "Action: Add User Name" control and click on the screen
  - Click "Lock" again This adds an action control to the screen which
    will cause the user name of the device to be added to each sighting
    as an attribute.

We've had several requests for this feature for cases where you would
like to be able to partition data by device name.

### 3.047 BETA: 02/26/2006

Bug fixes:

  - Cut/Copy/Paste caused crash when used from locked mode if control
    had been selected
  - Element select should not close on double click without valid
    selection
  - Moving map incorrectly calculates point position
  - Zoom Images/Moving map buttons should not appear over the image/map

### 3.046 BETA: 02/07/2006

Bug fixes:

  - Date/Time encoding fails if device reports \> 60 for seconds (which
    sometimes happens)
  - Crash on Palm device when control client is scaled below 1 pixel
  - GPS not detecting because EnumDevices doesn't enumerate GPS port
  - Client uninstall doesn't remove all files - fails on SmartPhone
  - Client taskbar sometimes becomes visible
  - Message and Fault window not properly scaled on high-DPI screens
  - Tutorial sequence on PocketPC should be removed: not useful
  - Client uninstall errors not logged
  - Message windows on Desktop can sometimes be hidden: crashes possible
  - Converting geo-referenced images to ECW should preserve
    geo-referencing
  - JPEG files not correctly recognized with Add Photo button
  - Palm: no users should generate error message
  - Remove shortcut keys from Sequence mode: confusing
  - Sequence Properties: GPS Timer doesn't work on Palm

New features:

  - Camera control. If you have a Windows Mobile 5 device with a camera,
    we have a new control that allows you to capture images directly.
  - Windows Mobile 5 is now fully supported.
  - MrSID images are now supported on both the desktop viewer and within
    the ECW converter tool.

### 3.040 BETA: 01/13/2006

Bug fixes:

  - Crash on load occasionally caused by race condition
  - Crash on map use after extended time

New features:

  - Option off "Sequence Properties" called "Use on GPS skip". If
    checked (on by default), then if you have a moving map assigned,
    pressing "Skip" will allow you to manually assign the GPS position
    for the sighting by pinpointing it on your map.
  - Option off "Sequence Properties" called "Sighting fix count". This
    allows customization of how many GPS points to take when acquiring a
    position. This improves accuracy at the expense of time.

### 3.039 BETA: 01/08/2006

Bug fixes:

  - Buttons do not invert correctly on all systems when pressed
  - SnapGPS action snaps even when editing a previously stored sighting
  - Manual GPS positions should not include accuracy when downloaded
  - GPS position is taken even when sighting already has a fix
  - State lost on save target screens when using "Retain state" feature
  - ConvertCTZ did not use XP themes
  - Initial directory not properly set on some editor dialogs
  - Merge sometimes leaves UI mode in closed state when viewing data
    files
  - Timer track export: file saved to the wrong directory and filename
  - Crash when viewing maps without layers
  - Timer tracks on maps should be ON by default

New features:

  - Major Target and Minor Target have been renamed to Save 1 and Save 2
  - Quit button is now in the top left corner
  - Edit button is now on the inspector button bar
  - Unsaved sightings is named "Unsaved" instead of 0-00:00:00
  - Sightings with 2D quality fix do not include Altitude
  - Sightings no longer display accuracy for manual sightings
  - The Moving Map control is now viewable in the GPS Viewer dialog
  - The Moving Map can be configured via a "Sequence Properties" dialog
    as can GPS timer and accuracy settings
  - CyberTracker includes a "Moving Map" converter for converting images
    in other formats to ECW
  - Map control has a "Flag" option which allows manual creation of GPS
    position for cases when no GPS fix is possible

### 3.037 BETA: 12/27/2005

Bug fixes:

  - Memos: text not always scrollable to the end
  - Palm: inverted colors don't always come out correctly
  - Crash when holding down "Skip" button during GPS acquistion
  - Palm: icons in tranparent list boxes are colored incorrectly
  - GPS Off icon does not have a line through it: inconsistent with
    Navigator representation
  - History control sometimes gets out of sync
  - Navigator skip screen button ocassionally displays incorrectly in
    the Designer
  - Data doesn't download when synchronizing to multiple computers
  - Database "Save As" doesn't handle all error conditions
  - Desktop application window size and position not saved between runs
  - Static elements sometimes have wrong icon
  - Deleting a screen doesn't always update the screen Preview window
  - "Element Columns" and "Sequence Profiles" should be separate dialogs
  - Export and Import directories not tracked properly
  - Import of data-only CTX files should default to "Report" mode
  - Import of data-only CTX files should validate Elements
  - Cut/Copy/Paste focus issues in Sequence Designer
  - Active Alias and Profile not tracked properly in "Test Run"
  - Overactive assert in Sighting Edit dialog
  - Lat/Lon precision in map view are too low
  - Vector Layers should not be the default tab in Map View Edit
  - Potential data loss when GPS reports high accuracy, but not a 3D fix
  - Cosmetic: region icon in map layers is malformed
  - CyberTracker Standard doesn't disable Sequence Design mode

New features:

  - File structure changed. CyberTracker originally kept a "Staging" and
    "Settings" folder in a per-user application data location. These
    have been moved to "My Documents\\My CyberTracker
    Databases\\System". The "System" folder is hidden, so you shouldn't
    see it. This has 3 main advantages: (a) To completely remove
    CyberTracker, just uninstall it and delete the "My CyberTracker
    Databases" folder. (b) The "Staging" and "Backup" directories will
    be easier to find if anything goes wrong. (c) Backing up "My
    CyberTracker Databases" will backup everything We have also created
    a "Maps" folder under "My CyberTracker Databases". If a map is
    placed in that folder, it will be accessible to anyone who shares
    your database as long as they have put the map in their own "Maps"
    folder.
  - New property: "Auto select index" which allows a default selection
    to be set on radio lists
  - New property: "Retain state" which allows the state of a screen to
    be retained between sightings
  - New property: "Save result" which allows a screen to be used for
    navigation only purposes without affecting the data in a sighting.
  - Number List now has "Minimum item width", "Columns" and "Auto select
    index" properties
  - Map View: If no image or other layers are present, then CyberTracker
    will use a world map as the default. This will automatically
    disappear when: (a) A valid image layer is added OR (b) One or more
    valid shape files are added OR (c) The projection is changed Map
    views now also support ER Mapper (ECW) files.
  - Timer track export. When exporting a shape file, timer tracks will
    also be exported. If your export shape file name is: "My Data.shp"
    then the timer tracks will be exported as "My Data\_line.shp". Both
    files have an additional data field which specifies the Id of the
    device that captured the data. This allows correlation between
    sightings and timer tracks.
  - New Control: Zoom Image. A new control that allows you to zoom and
    pan around high resolution images that are too large to fit on the
    screen.
  - CyberTracker Viewer. There is now a Viewer application, which is
    read-only for the database. You can view sightings and modify
    queries, but not save or modify the database in any way. It is
    available as a shortcut off the Start menu.
  - Add Photo button and Photo View There is an "Add Photo" button that
    makes it easy to bind sightings to images. The Photo view shows any
    photos in the currently selected sighting.
  - New Sample database: Feature demo A simple demo sequence that runs
    through some of the features of CyberTracker.
  - New Action: Add Attribute: allows the adding of data to a sighting
    without having to enter it on a screen. Useful for tagging sightings
    with meta-data.
  - New Action: Configure GPS: allows configuring the GPS timer and
    accuracy requirements without having to enter them on a screen.
    Useful when enforcing track timers and accuracy of readings.
  - New Action: Snap GPS: allows acquisition of GPS readings at specific
    places in a sequence, rather than always at the end. Useful for
    recording sightings from a fast moving vehicle, where you want the
    GPS reading to reflect the point where the observation was started.
  - New Control: Moving map. A new control allows the display of a
    realtime moving map on the device. This feature works on Windows
    Mobile/PocketPC devices only. We have no plans to support this on
    Palm. The map file must be in ECW (ERMapper) format. There is a free
    image converter for these files available at ERMapper. This control
    is not currently integrated into the GPS info screen.

### 3.035: 10/05/2005

Differences from === 3.021:

  - Improved Palm performance for older devices: CyberTracker now runs
    acceptably fast on devices as old as the original Handspring Visor.
  - Improved support for high resolution screens: this includes line
    doubling and better fonts. These options are available by setting
    the profile.
  - Improved installation mechanism: CyberTracker no longer requires
    manual uninstallation. When installing a new version, the previous
    version is automatically uninstalled.
  - The Icon library from version 2 has been included. These icons are
    stored as individual JPEG images in the Icons folder of the
    CyberTracker installation folder.
  - More GPS device support
  - Multiple improvements to UI controls including scrollbars, lists and
    icon history.
  - Bug fixes

### 3.033 BETA: 09/15/2005

Changes:

  - Key filter system allows filtering of large lists based on
    attributes.
  - The Wildlife sample now includes a demonstration of this new feature
    in the form of a Plant key. Note, the sample doesn't work very well
    on older Palm devices, because we are using high resolution color
    images. (Professional only until we create a template).
  - New check box style. (Professional only until we create a template).
  - New control: Element Image Grid. This control allows you to select a
    square on a grid for positional purposes, e.g. I'm in block C2\*
    Wildlife sample includes a demonstration. (Professional only until
    we create a template).
  - The Icon library from V2 is now included in the form of individual
    image files in the "Icons" folder of your CyberTracker installation
    folder.
  - Installation of Desktop now auto-uninstalls old version
  - Installation of PocketPC client now auto-reinstalls newer versions
  - Improved support for High DPI devices

### 3.026 BETA: 08/23/2005

Changes:

  - GPS Reading sometimes not taken (introduced in === 3.025)
  - Trimble Pathfinder GPS not always found
  - Prevent crash when writing templates to existing read only files
  - Improved support for High DPI devices: borders can be scaled
  - Support for 8 Images and 8 text fields per Element

### 3.025 BETA: 08/19/2005

Changes:

  - Pro version: new control "Element Container" designed to hold
    multiple Element Memo and Element Image controls
  - Bug Fix: After Synchronize links go blank
  - Bug Fix: CF GPS not recognized if inserted after CyberTracker
    started
  - Bug Fix: GPS waits until at least 2 sentences are read from the GPS
    before saving
  - Bug Fix: TSIP GPS device readings in wrong hemisphere
  - Improved About dialog

### 3.024 BETA: 08/15/2005

Changes:

  - Descriptions of properties below the property editor when editing
    sequences
  - Scroll bars now have up and down buttons on all controls, not just
    lists
  - GPS dialogs now show GPS state (i.e. detecting, acquiring, fix) on
    each tab
  - Bug fix: Crash when selecting a control when locked properties popup
    open
  - Bug fix: GPS satellite PRNs not correctly aligned

### 3.022 BETA: 08/03/2005

Changes:

  - Queried sightings are now pre-sorted by Date/DeviceId/Time
  - Optimized Palm support for older devices: performance is now
    comparable to version 2 when using the "Palm" profile
  - Scrollbars now have up and down buttons
  - The device up and down buttons on the bottom of the screen now
    function as "Page up" and "Page down" for lists
  - The device left and right buttons work as "Back" and "Next"
  - Compact Flash GPS devices, like the "Holux GPS Ultra" are now
    supported
  - Improved icon history list: requires any icon (32, 50, 100) to work
  - BUG Fix: Insufficient precision with shape file export of numbers

### 3.021: 07/20/2005

Changes:

  - Critical bug fixes
  - Support for PalmOS devices
  - Support for GPS tracks (positions taken at timed intervals)
  - Moving of sightings visually on the map view

History prior to 3.021 is not available.
