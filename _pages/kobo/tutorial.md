---
layout: page
title: Tutorial
nav_order: 2000
parent: KoBoToolbox
permalink: /kobo/tutorial
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
This tutorial shows how to use CyberTracker with KoBoToolbox. By the end, you will be able to use CyberTracker to capture data and view it on the KoBoToolbox backend.

## Requirements
- Windows (64-bit) or Mac
- Excel or other XlsForm editor
- Account on KoBoToolbox

## Steps
### 1. Create an account
Create an account on KoBoToolbox using the [sign-up flow](https://www.kobotoolbox.org/sign-up/).
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-1.png" /></td>
</tr>
</table>

### 2. Create a new Project
Create a new project using the **New** button. For more information, check out the [quick start guide](https://support.kobotoolbox.org/quick_start.html).
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-3.png" /></td>
</tr>
</table>

### 3. Adding questions
Create questions on the form using the **+** button. When done click **Save** and then **Deploy**. 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-4.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-5.png" /></td>
</tr>
</table>

### 4. Download, install and launch CyberTracker
Visit the [Download page]({{ site.baseurl }}/xlsform/download) and follow the instructions to install and launch CyberTracker. 

### 5. Connecting to the form
Download the form in CyberTracker by using the **Connect** page.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6a.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6b.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6c.png" /></td>
</tr>
</table>

### 6. Entering data
Tap on the Project name ('Tutorial') and then use the **+** button in the bottom right corner to add new data.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6d.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6e.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-6f.png" /></td>
</tr>
</table>

### 7. Submitting data
Tap on the **Submit** button in the bottom left corner. A confirmation dialog will popup. **Press and hold** the **Yes** button to confirm.
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-7a.png" /></td>
</tr>
</table>

### 8. Viewing collected data
Return to the KoBo web application and navigate to the **Data** tab. If it is disabled, refresh the page. Notice the submitted data is displayed. 
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-8.png" /></td>
</tr>
</table>

### 9. Open the `CTProjects` folder on the desktop
CyberTracker creates a folder on the desktop called `CTProjects`. Open this folder and navigate to the `Projects` sub-folder inside it. You will then see a folder for the Project you have just created. Open it and notice that it contains a file called `form.xlsx`.
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/tutorial-kobo-9.png" /></td>
</tr>
</table>

### 10. Open the form, make a change and save it
- Open `form.xlsx` and make a change. For example, add a new entry in the `choices` sheet, or a new question in the `survey` sheet. 
- Save the form

### 11. Reload the Project in CyberTracker
- Exit the Project by pressing the **Back** button in the top left corner
- Relaunch the Project by tapping on it
- Verify that the change that was made.

{: .warning }
Changes made to the form are not automatically uploaded to KoBo. You must re-upload the form to the backend when done.
