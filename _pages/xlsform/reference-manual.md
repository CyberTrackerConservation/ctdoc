---
layout: page
title: Reference manual
nav_order: 4000
parent: XlsForm extensions
permalink: /xlsform/reference-manual/
has_children: true
has_toc: false
---
CyberTracker XlsForm Reference Manual
========================
{: .no_toc }

Overview
--------
{: .no_toc }
CyberTracker is a universal data collection application which runs on mobile devices. One of the supported formats is [XlsForm](https://xlsform.org).

XlsForm has an [extension mechanism](https://xlsform.org/en/#advanced-use-and-extensibility) which allows users to activate CyberTracker behavior without affecting the semantics of the form.

This reference manual descibes the CyberTracker extensions. Note that XlsForms are simply an Excel files and the extensions are columns in the worksheets.

There are three kinds of customization:
- Views, e.g. grid styles for single and multi-select lists
- Behaviors, e.g. GPS track logs and save targets
- Developer code, e.g. a new widget

Backend
-------
{: .no_toc }
CyberTracker supports [ODK Central](https://getodk.org/), [KoBoToolbox](https://kobotoolbox.org) and [Survey123](https://survey123.arcgis.com). 

The CyberTracker extensions do not affect the semantics of the form and are transparent to backends. It is possible to use the same form to collect data across platforms (web, ODKCollect, etc) with a single form. In this scenario, CyberTracker would be chosen as a way to meet the needs of specific field workers.

Limitations
-------
{: .no_toc }
While CyberTracker supports most of the commonly used XlsForm features, it is not as mature as the existing data collection tools like ODK Collect, Kobo Collect and Survey123. Users should prefer to use those tools for mission critical projects.

<div style="page-break-after: always;"></div>

Table of Contents
{: .no_toc .text-delta }

{:toc}
- TOC

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-1.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-2.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-3.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-4.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-5.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-6.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-maps.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-7.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-8.md %}

<div style="page-break-after: always;"></div>
{% include_relative _reference-manual-faq.md %}

