---
layout: page
title: Getting started
nav_order: 100
parent: Tutorials
grand_parent: XlsForm extensions
permalink: /xlsform/tutorial/0
has_toc: false
---
Getting started
========================
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Purpose
This tutorial shows how to start working with CyberTracker XlsForm extensions. While they can be added to a form without going through this process, it is easier to test and validate them on a desktop before deploying to a mobile device.

## Requirements
- Windows PC (64-bit) or Mac
- XlsForm editor
- Account on a backend provider, e.g. KoboToolbox, ODK Central, Survey123

## Form template
[Download XlsForm]({{ site.baseurl }}/assets/xlsform/simple-form.xlsx)

## Steps
### 1. Create an account
- Create an account on your chosen provider. After signing up, you will have a username and password. 
- Create a new form or upload an existing form (see above for a sample).

### 2. Download, install and launch CyberTracker
Visit the [Download page]({{ site.baseurl }}/xlsform/download) and follow the instructions to install and launch CyberTracker. 

### 3. Install a project 
Connect to the form in CyberTracker and try it out. This is the flow in KoBoToolbox, but it is similar for other providers.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0a.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0b.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0c.png" /></td>
</tr>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0d.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0e.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0f.png" /></td>
</tr>
</table>

### 4. Navigate to the `CTProjects` folder on the desktop
CyberTracker creates a folder on the desktop called `CTProjects`. Open this folder and navigate to the `Projects` folder inside it. You will see a folder for the project you have just created. Open it and notice that it contains a file called `form.xlsx`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0g.png" /></td>
</tr>
</table>

### 5. Open the form, make a change and save it
- Open `form.xlsx` and make a change. For example, add a new animal in the `choices` sheet, or a new question in the `survey` sheet. 
- Save the form

### 6. Exit back to the Projects page in CyberTracker and then tap on your again to launch
Verify that the change that was made.

{: .warning }
Changes made to the form are not automatically uploaded to the provider. You must re-upload the form to the backend when done. If the form is updated, your changes will be overwritten. 
