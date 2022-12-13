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

## Goal
This tutorial shows how to start working with CyberTracker XlsForm extensions. By the end, you will be able to quickly make and test form changes within a desktop environment. This is generally much quicker and easier than deploying to a mobile device.

## Requirements
- Windows (64-bit) or Mac
- Excel or other XlsForm editor
- Account on KoboToolbox, ODK Central or Survey123

## Form template
[Download XlsForm]({{ site.baseurl }}/assets/xlsform/simple-form.xlsx)

## Steps
### 1. Create an account
- Create an account on your chosen provider. After signing up, you will have a username and password. 
- Create a new form or upload an existing form (see above for a sample).

### 2. Download, install and launch CyberTracker
Visit the [Download page]({{ site.baseurl }}/xlsform/download) and follow the instructions to install and launch CyberTracker. 

### 3. Install a project 
Download the form in CyberTracker by using the **Connect** page. The following is the flow using KoBoToolbox, but it is very similar for other providers.
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

### 4. Open the `CTProjects` folder on the desktop
CyberTracker creates a folder on the desktop called `CTProjects`. Open this folder and navigate to the `Projects` sub-folder inside it. You will then see a folder for the Project you have just created. Open it and notice that it contains a file called `form.xlsx`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-0g.png" /></td>
</tr>
</table>

### 5. Open the form, make a change and save it
- Open `form.xlsx` and make a change. For example, add a new animal in the `choices` sheet, or a new question in the `survey` sheet. 
- Save the form

### 6. Reload the Project in CyberTracker
Verify that the change that was made.

{: .warning }
Changes made to the form are not automatically uploaded to the provider. You must re-upload the form to the backend when done. If the form is updated, your changes will be overwritten. 
