---
layout: page
title: Web Update
nav_order: 15
parent: CyberTracker Classic
permalink: /classic/web-update/
---
# Web Update

Web Update is a way to distribute CyberTracker applications over the web. This reduces the need to connect with a USB cable to install and update apps.

![]({{ site.baseurl }}/assets/classic/WebUpdate.png)

**Edit Application dialog**

## Concepts

An update consists of two files: a DEF and a ZIP. The DEF file is a small text file which contains a version and a  web link to the ZIP file. The ZIP contains the application along with any offline maps. The mobile app reads the DEF file for initial installation and for update checks.

## Initial setup using file hosting (advanced)

If the web location where these files will be hosted is known, then the process is straighforward:
1. On the CyberTracker desktop application, open the "Edit Application" dialog and go to the "Web Update" tab.
2. Enter the URLs for the DEF file and the ZIP file and click "Publish".
3. Copy the newly created files (CTApp.def and CTApp.zip) from the "CT" folder on the desktop to the file host.
4. On the mobile application, go to the Connect page, then select the CyberTracker connector, then Web Install. Enter the DEF link and the app will be installed.
5. See the section below on sharing the link in a more user friendly way.
6. Remember to save the database, so in future you know where the link and def file are.

## Initial setup using Google Drive or Dropbox

1. Login to Google Drive or Dropbox and create a new folder. The name does not matter.
2. On the CyberTracker desktop application, open the "Edit Application" dialog and go to the "Web Update" tab. Click the “Publish” button. This creates a “CT” folder on the desktop. Open this folder in Windows Explorer by double clicking on it. Note that the property settings on the dialog do not matter at this point.
3. Drag CTApp.def and CTApp.zip to the newly created folder in your browser.
4. Right click on CTApp.def in the browser and select “Copy link”. On Google Drive change “General Access” to “Anyone with the link” and click “Copy link”. Paste the link into CyberTracker in the “DEF file URL” property. 
5. Right click on CTApp.zip in the browser and select “Copy link”. On Google Drive change “General Access” to “Anyone with the link” and click “Copy link”. Paste the link into CyberTracker in the “ZIP file URL” property. 
6. Click “Publish” again in CyberTracker. Drag the CTApp.def and CTApp.zip files from the desktop CT folder into the browser and overwrite the existing ones. On Google Drive, make sure to choose overwrite, rather than create copies. This is to prevent the links from changing.
7. On the mobile application, go to the Connect page, then select the CyberTracker connector, then Web Install. Enter the DEF link and the app will be installed.
8. Remember to save the database, so in future you know where the link and def file are.

## Subsequent updates

1. On the CyberTracker desktop application, open the "Edit Application" dialog and go to the "Web Update" tab. Click the “Publish” button.
2. Replace the files on Google Drive, DropBox or the file server with the newly created DEF and ZIP from the “CT” folder on the desktop.
3. CyberTracker Mobile will recognize an update and offer to install it.

## Sharing
1. On the CyberTracker mobile app, long press on the project to bring up the Project details screen.
2. Tap the “QR Code” option. Share the link or the QR code with others. If CyberTracker is not installed on the device, then the user will be prompted to install it. If it already installed, then the project will be immediately downloaded and installed.

## AB Testing

The "Tag" property can be surfaced in the collected data. To enable this, enter Layout mode, select "Actions" from the Toolbox on the right and place an "Add Attribute" action on the first screen. Set the "Result Element" and then check the "Update tag" property. This causes the system to add an attribute to sightings with the value of the tag property in the DEF file.

By sending different DEF links to different users, it is possible to label user data according to which DEF file link they used to install the application.
