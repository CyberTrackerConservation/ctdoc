---
permalink: /docZ/
layout: default
search_exclude: true
nav_exclude: true
---


1 Introduction
In 2021, the Caring for Country (CfC) Branch recognized the high priority of designing an Integrated Monitoring and Evaluation framework for NLC Ranger Groups and support staff. This framework aimed to implement a regional approach to Monitoring, Evaluation, Reporting, and Improvement (MERI) to enhance workflows, decision-making, and reporting across the CfC unit. The MERI framework falls under the Adaptive Management (AM) framework family, which is crucial for managing complexity and uncertainty.

Defined as "a structured, iterative process of robust decision-making in the face of uncertainty, with an aim to reduce uncertainty over time via system monitoring," the AM framework serves as a valuable tool for understanding and adapting systems. Given the urgency of many environmental issues, it is essential to take action now while remaining open to adaptation if assumptions and strategies do not yield the desired outcomes.

The AM Framework provides guidance in determining the effectiveness of actions, selecting between alternatives, and testing underlying assumptions. In NLC, the Land and Sea Department will apply the AM Framework through the Caring for Country (CfC) Adaptive Management Framework. The CfC unit has adopted Healthy Country Planning (HCP), an adaptation of the Conservation Standards (CS), to provide a standardized framework for adaptive management plans. The consistent structure of the CS/HCP ensures that information from individual adaptive management projects can be consolidated regionally, forming the basis for the CfC's MERI platform.

As part of the "NIAA Project Schedule � Indigenous Ranger Grants � Jobs Land and Economy Programme," the CfC Branch has secured funding for 6.5 years for the "Acquisition of new and emerging technology, including the development and implementation of a Project, Environmental, and Cultural Information Management System across Ranger Groups," also known as the "CfC Adaptive Management Framework" (CfC AM Framework). This framework is integrated within the AM methodology and processes at all CfC branch levels, encompassing both Ranger groups and Program support.

1.1 Adaptive Management Cycles
Adaptive management encompasses various methodologies, yet all share six fundamental elements:
1- Assessing (A)� Program Logic encompasses determining targets/values, threats, result chains to lay a solid foundation.
2- Planning (P) - Formulating operational, monitoring, and work plans to ensure a well-structured approach. Determining strategies and activities.
3- Execution and Monitoring (M) - Carrying out plans while collecting data on activity progress, threat reduction, and target improvements through various indicators.
4- Evaluation (E) - Analysing collected data, gauging program success, and identifying areas for improvement to enhance overall performance.

5- Reporting and Sharing (R) - Disseminating information, including achievements and lessons learned, to foster transparency and collaboration.
6- Improvement (I) - Utilizing insights from the gathered information to refine processes and update the Program Logic, thereby promoting continuous enhancement.








For each of the six steps in the Adaptive Management cycle (Assessment, Planning, Monitoring, Evaluation, Reporting, and Improvement), successful implementation necessitates:
- External consultancy support for Program Logic design and integration
- Software development of the CfC AM Portal
- Hardware integration for field data collection, including procurement and testing

The design and implementation of the CfC AM Framework proceed in a chronological sequence on two levels:
1- Framework Component design, implementation, deployment, and testing:
a. Program Logic (HCP + Miradi � cloud-based)
b. Activity Scheduler & Tracker (hosted within the CfC AM Portal)
c. Field data collection (Quantitative - cloud-based)
d. Field data collection (Qualitative - TBD)
e. Dashboards (PowerBI - hosted within the CfC AM Portal)
f. Artificial Intelligence (AI) (LLM trained on CfC Data � with prompt - hosted within the CfC AM Portal)
g. Reports (Milestone reports - hosted within the CfC AM Portal)
      h. Export (Data Governance - administered within the CfC AM Portal) 2- Ranger groups joining the framework:
a. HCP operationalization and Miradi project fine-tuning
b. Deployment (Activity Scheduler & Tracker, Reporting, Field data collection, and Export)
c. Testing
d. Support

By following this structured approach, the CfC AM Framework can be effectively designed, implemented, and integrated, ensuring that the participating Ranger groups receive the necessary tools and support to optimize their Adaptive Management efforts.

2 CfC Tool Set
CfC has selected key tools for the development of the AM Framework:

Name
 Type of Software
Tools
AM
Element
Purpose
Location
Logo
Miradi
Program
Logic Management
A, P, I
Design Program
Logic for each project
Cloud-based

SMART
(Cyber Tracker and Fulcrum are also possible options)
Field Data Collection
M
Collect land management field data
Cloud-based


iAuditor
Field Data Inspection
M
Collect WH&S
and Compliance field data
Cloud-based


Garmin inReach
GPS Tracking
M
Fleet and people GPS tracking
(WH&S and SAR)
Cloud-based


Mix
Telematics
GPS Fleet
Tracking
M
Track Vehicle
Cloud-based


Activity Scheduler & Tracker
Activity Planning and Tracking
M
Plan and track daily work plan
CfC Portal

 
PowerBI
Dashboard
E, R
Develop Dashboards
CfC Portal

Report
Report
forms
E, R
Finalise report
CfC Portal

Artificial Intelligence
AI Prompt
E, R
Train LLM with CfC Data
CfC Portal

Export
Data Export
R
Provide data export to external stake
holders (APIs)
CfC Portal


2.1 Miradi � Program Logic
The program logic embedded within each Miradi project serves as the fundamental framework that directs the rangers' efforts. Every individual "Miradi Project" comprises multiple "Miradi Result Chains," each of which consists of several "Miradi Strategies." In turn, each "Miradi Strategy" encompasses numerous "Miradi Activities."

Situation Assessment Example:



Result Chain example:

Activity list example:

A Miradi Activity, such as "Spray Gamba Grass" or "General Boat Patrol," may be carried out multiple times throughout the year. As a result, a parent-child relationship exists between the "Miradi Activity" in Miradi and the "Tracked Activity" in the " Activity Scheduler and Tracker" (AST)
The "Miradi Activity" serves as the parent, with multiple "Tracked Activity" instances functioning as its children.






Miradi serves as the primary source of information for the data associated with an Activity. A Miradi Activity includes attributes that are passed down to its children when a "Tracked Activity" is generated within the "Activity Scheduler & Tracker."


Those Attributes are stored in the Miradi Task attached to the Miradi Activity.





2.1.1	Project level Miradi information transfer
Project level information is also transferred from Miradi to the Activity Tracker. Each Miradi project contain an extra Result Chain call �SEETINGS�

WHO
list of staffs (active and inactive) members of the project
FLEET
list of vehicles (active and inactive) available for the project
COMMS
list of communication equipment (active and inactive) available
for the project
GPS TRACKER
list of GPS Tracker equipment (active and inactive) available for
the project
SAR LEVEL ONE PHONE LIST
list of phones to send a text to if SAR escalation level 1 is
activated
SAR LEVEL ONE EMAIL LIST
list of email addresses to send a message to if SAR escalation
level 1 is activated
SAR LEVEL TWO PHONE LIST
list of phones to send a text to if SAR escalation level 2 is
activated
SAR LEVEL TWO EMAIL LIST
list of email addresses to send a message to if SAR escalation
level 2 is activated
SAR LEVEL THREE PHONE LIST
list of phones to send a text to if SAR escalation level 3 is
activated
SAR LEVEL THREE EMAIL LIST
list of email addresses to send a message to if SAR escalation
level 3 is activated

See Appendix E for an example of a Miradi extract of the �Details� field in the �SETTINGS� result chain.

The program logic components of each project, including Result Chains, Strategies, and Activities, can be accessed through the Miradi API. (https://miradishareapiv1.docs.apiary.io/#)

https://www.miradishare.org/ux/home

2.2 SMART � Land Management Field Data Collection

The SMART platform consists of a set of software and analysis tools designed to help conservationists manage and protect wildlife and wild places. SMART can help standardize and streamline data collection, analysis, and reporting, making it easier for key information to get from the field to decision-makers.

SMART supports a broad range of conservation management activities, including biodiversity conservation, law enforcement, tourism and visitor management, natural resources use, intelligence, and performance and threat level assessments.

Each Ranger group has a SMART account that enables them to collect conservation management data using various apps on handheld smart devices.



 


The field data collected can be accessed through the SMART API. https://smartconservationtools.org/
2.3 iAuditor � WH&S Field Data Collection

Each Ranger group has an iAuditor account that enables them to carry out inspections on vehicles and assets, as well as collect Compliance and WH&S data via various apps.



https://safetyculture.com/iauditor/

The field data collected can be accessed through the Safety Culture API (https://developer.safetyculture.com/)


2.4 Garmin inReach � GPS Tracking

Garmin inReach is a series of satellite communication devices produced by Garmin. These devices allow users to send and receive text messages, track their location, and request assistance in case of an emergency from anywhere in the world, as long as there is a clear view of the sky. The inReach devices use the Iridium satellite network to provide two-way communication, even in remote or off-the-grid locations where cellular coverage is not available.

In the event of a search and rescue (SAR) operation, it is crucial to know the precise location of the rangers to coordinate an effective response. The goal is to provide a real-time overview of the current and historical whereabouts of each ranger and their corresponding vehicle.


https://discover.garmin.com/en-GB/inreach/personal/

The GPS positions and tracks can be accessed through the Garmin Connect API (https://developer.garmin.com/inreach-portal/overview/)

2.5 Mix Telematics � GPS Fleet Tracking

The NLC is utilising Mix Telematics to monitor its fleet, which involves meeting similar requirements for providing real-time and historical location data for each vehicle.


https://mixtelematics.com/eu/
API: https://explore.mixtelematics.com/mix-integrate

3 Development
3.1 Scope

The primary objective of this project is to design and implement an innovative adaptive management portal (CfC Portal) that serves as a comprehensive solution for effective data integration and management.
The portal comprises six key internal components:
- "Activity Scheduler and Tracker" for scheduling and monitoring Activities (Input & Output)
- "Dashboard" for visualizing and summarizing data
- "Report" to report on contract milestones
- �Artificial Intelligence� to interrogate the CfC LLM trained on CfC data
- "Export" component for sharing information through APIs
- �Settings/Administration� for users and general settings administration

Utilising a data lake for storage, the portal seamlessly connects and harmonizes data from multiple external sources, such as Program Logic "Miradi", Field Data Collection (SMART Conservation), iAuditor (WH&S Inspections), GPS tracking devices (Search and Rescue) and other systems.

The adaptive management portal not only ingests and manages data from these external components, but also from its own internal components (Activity Scheduler and Tracker, Reports), offering a unified platform for data handling.
Access to this valuable data is made available to both internal and external stakeholders through intuitive dashboards and reports (PowerBI), AI prompt, ensuring efficient collaboration and decision-making.
In addition, the project places a strong emphasis on data governance, data sovereignty, and intellectual property to guarantee secure and responsible data management practices (Export component).


3.2 Spaces and Projects

The CfC Portal is designed to host multiple "Spaces," each dedicated to a specific CfC project that requires a platform for storing, managing, and visualising adaptive management data. A Space grants Rangers (from a particular ranger group) and support staff access to:
- The Activity Scheduler and Tracker component
- The Dashboard/Reporting component
- The Export component
- The Settings/Administration component

In terms of external, cloud-based components, each ranger group operates its own project, which comprises:
- A Program Logic stored within a specific Miradi project hosted on the Miradi Share platform
- A Field Data Collection SMART project hosted on the SMART Conservation platform
- A WH&S iAuditor project hosted on the iAuditor platform
- A Garmin GPS tracker project hosted on the Garmin inReach platform
- A Fleet GPS tracker project hosted on the Mix Telematics platform
- Additional external components that may be added in the future

3.3 User Interface

3.3.1 Access
CfC staff members, depending on their roles and responsibilities, will have access to one or multiple Spaces inside the CfC Portal. For instance, a Ranger Coordinator will only have access to their own ranger group's Space, while a Regional Coordinator will have access to four or five Spaces (one for each ranger group in their region). A Manager will have access to all Spaces. User management (account credentials) for each Space is handled by the Settings/Administration component.










3.3.2 Activity Scheduler and Tracker
By clicking the AST button within a designated Space, users will be directed to the AST Home page, which features both a Calendar view and a List view displaying all previously entered activities. To edit an activity, simply click on the desired item either in the calendar or the list.



To create a new activity, users simply need to click the "Create Activity" button, opening an empty activity form ready for completion.
The user interface specifications for the Activity form can be found in Appendix B and Appendix C.
A search function will enable users to search for activities based on any of the activity fields.

3.3.3 Reports
Milestone reports are an essential requirement for contracts (such as NIAA, Fee for Services, etc.). Rangers and support staff will have access to the Reports component, which allows them to complete the necessary form for each individual report or milestone.
A specific form will be created for each milestone attached to the contract. This component will be modelled on the Learning on Country M&E Portal. UI and workflows to be determined.

3.3.4 PowerBI
By clicking the PowerBI button within a designated Space, users will be directed to the PowerBI Dashboard Home page for the specific Space.
The contents and user interface for the PowerBI Dashboard are provided in Appendix D.

3.3.5 Artificial Intelligence (AI)
The aim is to provide a prompt access to the CfC LLM trained on all the data collected by the CfC portal (internal and external components).
UI to be determined.

3.3.6 Export
The Portal enables access to raw data via a series of APIs. External stakeholders will receive access keys (tokens) that grant them permission to access raw data for storage within their own databases or systems. For instance, the NT Weed Branch may access the weed data gathered by rangers, contingent on the terms of their agreement and contract. Robust data governance is crucial for the proper functioning of this component.


3.3.7 Administration/Settings
3.3.7.1 Portal level 
The overall portal Administration and Settings will be consolidated on a dedicated page, encompassing user management, general settings, export configurations, access controls, data governance, and more.


3.3.7.2 Space level 
Each Space will have its own dedicated Administration and Settings page where the creation of new Spaces will be managed. For the AST to function, a link to the specific Miradi project API is required. Additionally, links to external field data collection components (such as SMART, iAuditor, inReach, etc.) are necessary for the PowerBI and Export components to operate effectively.



3.4 Activity Workflows

3.4.1 Introduction
Parent activities are initially planned within Miradi using the Workplan module.
The Workplan module offers the flexibility to plan parent activities on different timescales - daily, weekly, monthly, and quarterly. For the ranger activities, we have chosen to plan them on a quarterly basis.




To streamline the process of scheduling Miradi's planned activities, the CfC Portal has an integrated �Activity Scheduler and Tracker� component. This component is essential for the ranger coordinator to efficiently schedule and track child activities.

The Activity Scheduler and Tracker home window is divided into three main sections:
Left Pane: This section displays a list of Miradi's parent activities. The list can be filtered in multiple ways, such as by showing all activities, activities per quarter, or by using the search function. This allows the ranger coordinator to quickly find and select the required parent activities.
Right Pane - Top: This section features a calendar view of the scheduled child activities. The calendar view provides a visual representation of the activities scheduled over time, making it easy for the ranger coordinator to identify any potential scheduling conflicts or gaps.
Right Pane - Bottom: This section presents a list view of the scheduled child activities. This format offers a more detailed look at the scheduled activities, including important information such as dates, times, and locations.



3.4.1.1 Miradi Activities View Filtering 
The left pane displays the available parent Miradi activities, organized using the "Result Chain" / "Strategy" / "Activity" hierarchy in a folder/subfolder format. Users can easily filter the list of activities presented by utilizing the filtering options located above the pane:
"All Activities" checkbox: Selecting this option will display all activities from the Miradi project.
"Current Quarter Miradi Activities" checkbox: When checked, only activities from the current quarter will be shown.
"Next Quarter Miradi Activities" checkbox: Selecting this option will display activities from the upcoming quarter.
"Search" text box: This feature allows users to display activities with a name that matches the text entered in the search box.

These filtering options enable users to quickly and efficiently locate the desired Miradi activities, making it easier to manage and schedule tasks within the Activity Scheduler and Tracker.

3.4.1.2 Creating child scheduled activities 
To create child scheduled activities, there are two methods available:
Drag and Drop: The ranger coordinator can simply drag a parent Miradi activity from the Left Pane and drop it onto the desired date in the Top Right Pane (calendar view). This will automatically create a child scheduled activity for the selected parent activity on the specified date.
Create Scheduled Activity Button: The ranger coordinator can also click the "Create scheduled activity" button, which will prompt them to select a parent Miradi activity, specify a date and time, and add any additional information required. Once submitted, the new child scheduled activity will appear in both the calendar view and the list view.

By having a clear and user-friendly interface for the �Activity Scheduler and Tracker�, the ranger coordinator can effectively manage Miradi's planned activities, ensuring that critical activities are scheduled and tracked in a timely manner.

3.4.1.3 Editing scheduled activities 
To edit a schedule activity, the user can double click on a scheduled activity in the calendar view or in the list below.

3.4.2 Workflow


3.4.2.1 Standard 
Every morning, the rangers hold a "Toolbox" meeting to finalise the day's plans. They determine the involved personnel, location, vehicles, communications, personal GPS trackers, and the time for setting the SAR alarm for each activity. If the planned activities are already in the AST, each activity is reopened, and the required information is added. If a new activity is required, it is created in the AST.

NO ground activity can start without the Tracked Activity being �Active� in the AST.
The required fields for activation are the parent Miradi Activity, What, When, SAR alarm time, Where, Vehicle, Comms, Personal GPS Trackers, and a completed Pre-Requirements checklist.

After completing an activity, the ranger team informs the coordinator of the activity's outcome, and the SAR alarm for each Tracked Activity is turned off. The AST is updated with the necessary information for each activity. The Tracked Activity remains "Active" until all post-completion fields are entered, including the incident report (if no incident, �No incident� must be entered), and a Post-Requirements checklist is completed. Only then, the activity status can be changed to �Complete�.

3.4.2.2 Workflow exception � TA Cancellation 
A TA can be cancelled before its Activation (status �Planned�), after its Activation (status �Active�) or if its status is �Overdue�. In any case, a reason must be given for the cancellation. The SAR alarm is automatically turned off after the cancellation.

3.4.2.3 Workflow exception � TA Overdue 
If the planned date for a Tracked Activity has passed, its status changes to "Overdue." The activity can be re-planned for a new date or cancelled.

3.4.2.4 Workflow exception � SAR Alarm activated 
If the SAR alarm is not turned off within a specific time frame, the TA status changes to �Alarm� and an escalating series of text messages and emails will be sent to coordinators level one at SAR time), support teams (level two, X minutes after SAR time), and management and WHS teams (level three, Y minutes after SAR time).

The list of contact information and delay times between alarm levels is managed in the Settings/Administration component of the portal.

3.4.2.5 Activities lasting more than one day 
It is possible that an activity lasts more than one consecutive day if located in a remote location away from the ranger base (remote cultural camp, survey, controlled burn, �). In this case, the SAR alarm will be automatically reset each morning during the activity period.

3.4.2.6 Activities in remote location without internet access 

If rangers are working in remote locations without internet access, they will contact their Regional project officer/coordinator each morning via satellite phone to enter the required information into the AST and activate the Tracked Activity. Upon returning to the base, the rangers will provide updates to the support staff, who will turn off the SAR alarm and update the AST. The Tracked Activity can be completed once the rangers return to the base.

See appendix A for workflow example.
See appendix B for user interface at all stages.
See appendix C for the Tracked Activity User interface form (fields details)

3.4.3 Tracked Activity Status Life Cycle








3.5 General System Requirements

3.5.1 Data residency and security requirements
The requirements are available on the ACSC website:
https://www.cyber.gov.au/acsc/view-all-content/publications/anatomy-cloud-assessment- and-authorisation

3.5.2 Portability / Open Source
The development of the CfC portal has the potential to benefit other non-NLC ranger groups. Consequently, maintaining the entire project as open-source and easily portable to another cloud instance is a crucial requirement.

3.5.3 Scalability
Initially (within 6-12 months), the portal will contain three to four projects (Mardbalk Rangers, Bulgul Rangers, Malak Malak Rangers, and CfC Support). However, it is expected to expand to twelve to fifteen projects in the coming years. Ensuring that adding new projects to the portal requires minimal configuration and is as automated as possible (API connections to external systems, etc.) is of utmost importance.

3.5.4 Data Lake: All DB � SAL aas
Copy / Synchronisation of all external data in the CfC data lake:
- Miradi
- SMART
- iAuditor
- inReach
- Mix Telematics

3.5.5 Platform
The portal should be easily accessible via a web browser on a variety of devices, including smartphones, tablets, and standard desktop computers.

3.5.6 Documentation
Users and technical documentation is required.

4 Appendix
4.1 Appendix A � Activity Life Cycle



4.2 Appendix B � Activity Scheduler and Tracker UI specifications










4.2.1	Miradi Activity update
If a Tracked Activity has its Miradi Activity changed, this will have an impact on the fields imported from Miradi (SAR, Contract, Finance, Pre-Requirements and Post-Requirements). As a result, a clear message should prompt users for confirmation if the Tracked Activity is linked to a different Miradi Activity. Note that this operation is not permitted while the Tracked Activity is in an "Active" state.







Caring for Country Adaptive Management Portal	31

4.3 Appendix C � Activity Scheduler and Tracker form specifications

Field Name
Data Type
Data Source/ Drop Down List Values
Comment




Activity
Miradi Activity
Miradi Program Logic (API / Data Lake)
Connect to Miradi and select: 1) Result Chain; 2) Strategy and 3) Activity;
What
Free text
User
Activity Name
[Required for Saving/Activate/Complete]
When
* Start Date-Time
* End Date-Time
Free text Editable
User
Start Date is a mandatory field; Can reset time fields as required; can enter future or past dates.
[Required for Saving/Activate/Complete]
SAR Alarm
Editable
User
Inherit from Miradi if required or not
If required, the user must enter a time (will not activate if the time has not been changed)
Where
Free text
Editable
User
Locations(s) of activity
[Required for Activate/Complete]
Who
Select
Multiple choice
List of staff for Ranger Base
List provided by the Miradi API � Project level � in Data lake
Fleet
Select
Multiple choice
Vehicle List for Ranger Base
List provided by the Miradi API � Project level � in Data lake
Comms
Select
Multiple choice
Comms List for Ranger Base
List provided by the Miradi API � Project level � in Data lake
GPS Tracker
Select
Multiple choice
Personal GPS Tracker List for Ranger
Base
List provided by the Miradi API � Project level � in Data lake
Contracts
Free text
Editable
Miradi Program Logic (API / Data Lake)
Pre-filled from Miradi API Task <CONTRACT>
Finance
Free text
Editable
Miradi Program Logic (API / Data Lake)
Pre-filled from Miradi API Task <FINANCE>
Incidents
Free text
Editable
User
List the incidents of the day
Notes
Free text


Attachments
Browse




Photos
Browse

Store GPS metadata stored for photos so that they can be shown spatially
Pre-Requirements
checklist
Ticking boxes
Miradi Program Logic (API / Data Lake)
Pre-filled from Miradi API Task <PRE>
Post-Requirements
checklist
Ticking boxes
Miradi Program Logic (API / Data Lake)
Pre-filled from Miradi API Task <POST>
Running Sheet
Module
User

The running sheet allow the creation and management of multiple sheets with the following field:
- Sheet creation date and time
- �What�: Description field (Text)
- Comments/Notes (Text)
- Attached files
Logs
Multiple texts Not editable
Automated
Date creation of the activity Username creator
Last update of the activity Username of last update
SAVE
Button
User
The activity is saved if it contains the minimum requirement for saving
CLOSE
Button
User
Close the activity without saving (if the activity has been modified, give option to
save)
PRINT
Button
User
Print the activity with all its fields
ACTIVATE
Button
User
The activity is activated if the required conditions for activation are satisfied
COMPLETE
Button
User
The activity is complete if the required conditions for completion are satisfied
CANCEL
Button
User
The activity is cancelled � a reason for cancellation is required
The activity stays in the Calendar/List
Cancelled Reason
Select
User
Only required if Status = Cancelled List of standard reasons
Compulsory free text if �Other� is selected�
Please see standard reasons
DELETE
Button
User
Only �Planned� Activity can be deleted




Caring for Country Adaptive Management Portal	33

4.4 Appendix D � PowerBI dashboard specifications

The PowerBI dashboard(s) present the data available from all the components of the framework:
a. Program Logic (Miradi)
b. Activity Scheduler & Tracker
c. Field data collection (SMART, iAuditor, Inreach, �)






4.5 Appendix E - Miradi extract of the �Details� field in the �SETTINGS� result chain
WHO>
<ID>Xavier Espiau</ID><ACTIVE>1</ACTIVE>
<ID>Justin Allen</ID><ACTIVE>1</ACTIVE>
<ID>Mike Carmody</ID><ACTIVE>0</ACTIVE>
<ID>Charmaine Miningirrgirr</ID><ACTIVE>1</ACTIVE>
<ID>Mardbalk Ranger Coordinator</ID><ACTIVE>1</ACTIVE>
<ID>Peter Phillips</ID><ACTIVE>1</ACTIVE>
<ID>Roy Winunguj</ID><ACTIVE>1</ACTIVE>
<ID>Karen Jimara</ID><ACTIVE>1</ACTIVE>

<ID>Phillip Nargarriba</ID><ACTIVE>1</ACTIVE>
<ID>Nicholas Hunter</ID><ACTIVE>1</ACTIVE>
<ID>Rasltin Djorlom</ID><ACTIVE>1</ACTIVE>
<ID>Audrey Mardbinda</ID><ACTIVE>1</ACTIVE>
</WHO>

<FLEET>
<ID>NLC-100</ID><TYPE>Car Toyota 4WD</TYPE><ACTIVE>1</ACTIVE>
<ID>NLC-115</ID><TYPE>Car Highlux 4WD</TYPE><ACTIVE>1</ACTIVE>
<ID>NLC-165</ID><TYPE>Car Troopy 4WD</TYPE><ACTIVE>0</ACTIVE>
<ID>Quad #1</ID>Quad Honda 4WD<TYPE></TYPE><ACTIVE>1</ACTIVE>
<ID>Quad #2</ID><TYPE>Quad Yamaha 4WD</TYPE><ACTIVE>1</ACTIVE>
<ID>Tiny #2</ID><TYPE>Boat Tiny 4WD</TYPE><ACTIVE>1</ACTIVE>
</FLEET>

<COMMS>
<ID>Sat #1</ID><NUMBER>+61487987589</NUMBER><TYPE>Sat phone</TYPE><ACTIVE>1</ACTIVE>
<ID>Sat #2</ID><NUMBER>87458964548</NUMBER><TYPE>Sat phone</TYPE><ACTIVE>1</ACTIVE>
<ID>Sat #3</ID><NUMBER>1578459547</NUMBER><TYPE>Sat phone</TYPE><ACTIVE>0</ACTIVE>
<ID>Mob Ranger Coordinator</ID><NUMBER>+6142584789585</NUMBER><TYPE>Mobile phone</TYPE><ACTIVE>1</ACTIVE>
<ID>Mob #1 </ID><NUMBER>+6145987231548</NUMBER><TYPE>Mobile phone</TYPE><ACTIVE>0</ACTIVE>
</COMMS>

<GPS_TRACKER>
<ID>InReach #1</ID><NUMBER></NUMBER><TYPE>GPS TRACKER</TYPE><ACTIVE>1</ACTIVE>
<ID>InReach #2 </ID><NUMBER></NUMBER><TYPE>GPS
TRACKER</TYPE><ACTIVE>1</ACTIVE><ID>InReach #5
</ID><NUMBER></NUMBER><TYPE>GPS TRACKER</TYPE><ACTIVE>0</ACTIVE>
</GPS_TRACKER>

<SAR_LEVEL_1_PHONE>
<NUMBER>0437793228</NUMBER>
<NUMBER>0889548789</NUMBER>
</SAR_LEVEL_1_PHONE>

<SAR_LEVEL_1_EMAIL>
<EMAIL>esipax@nlc.org.au</EMAIL>
<EMAIL>mardbalkrc@nlc.org.au</EMAIL>
<EMAIL>mardbalk@nlc.org.au</EMAIL>
</SAR_LEVEL_1_EMAIL>

<SAR_LEVEL_2_PHONE>
<NUMBER>0437793228</NUMBER>
<NUMBER>0889548789</NUMBER>
</SAR_LEVEL_2_PHONE>

<SAR_LEVEL_2_EMAIL>
<EMAIL>esipax@nlc.org.au</EMAIL>
<EMAIL>mardbalkrc@nlc.org.au</EMAIL>
</SAR_LEVEL_2_EMAIL>

<SAR_LEVEL_3_PHONE>

<NUMBER>0437793228</NUMBER>
<NUMBER>0889548789</NUMBER>
</SAR_LEVEL_3_PHONE>

<SAR_LEVEL_3_EMAIL>
<EMAIL>esipax@nlc.org.au</EMAIL>
<EMAIL>mardbalkrc@nlc.org.au</EMAIL>
</SAR_LEVEL_3_EMAIL>












