---
layout: default
title: XlsForm
has_children: true
nav_order: 6000
permalink: /xlsform/
---
# XlsForm

## What is 'XlsForm'?
[XlsForm](https://xlsform.org) is a form standard created to help simplify the authoring of forms in Excel. Authoring is done in a human readable format using a familiar tool that almost everyone knows - Excel. XLSForms provide a practical standard for sharing and collaborating on authoring forms. They are simple to get started with but allow for the authoring of complex forms.

## How does it relate to CyberTracker?
CyberTracker supports the XlsForm form standard and connects to popular backends: [ODK Central](https://getodk.org/), [KoBoToolbox](https://kobotoolbox.org) and [Survey123](https://survey123.arcgis.com). CyberTracker Online will also use XlsForm.

CyberTracker works like other mobile XlsForm data collection tools, but adds a layer of customization. This layer makes it easy to add new appearances and behaviors. For example: save targets, location tracks, theme colors, grid styles and more. Entirely custom layouts and workflows can be created without modifying CyberTracker. 

CyberTracker only affects how data is collected, not what is collected. It is transparent to the chosen backend and the form will continue to work in other tools.

## What is the workflow?
1. Design an XlsForm in Excel
1. Add `ct="http://cybertracker.org/"` to the namespaces column in the **settings** sheet
1. Add a column titled `bind::ct:parameters` to the **settings**, **survey** and **choices** sheets
1. Create JSON and place it in this column to activate the desired behavior
1. Upload the form to the desired backend and publish it
1. Connect with CyberTracker, download the form and collect data
1. Tap 'Submit' to upload data

## When should CyberTracker _not_ be used?
While CyberTracker supports most of the commonly used XlsForm features, it is not as mature as the existing data collection tools like ODK Collect, Kobo Collect and Survey123. Users should prefer to use those tools for critical projects.
