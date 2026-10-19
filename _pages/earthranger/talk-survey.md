---
layout: page
title: Talk survey
nav_order: 1
parent: EarthRanger
grand_parent: Connectors
permalink: /earthranger/talk-survey/
---
# Talk survey
{: .no_toc }

A talk survey is a hands-free way to collect EarthRanger events. The observer walks or drives a route and simply talks: CyberTracker records what is said, transcribes it, splits it into observations, fills in the event fields from the words, and submits each observation to EarthRanger as an event. Nothing is typed in the field.

- TOC
{:toc}

## How it works

A talk survey is built from one EarthRanger event type. Every record it creates is an event of that type.

### A survey is a session

1. **Start.** The observer enters the start location and any *metadata fields* (for example, transect, team or vehicle), then presses **Start survey**. CyberTracker writes a *Start* record and begins logging a GPS track.
2. **Talk.** The voice recorder runs continuously. Each spoken utterance is saved as a clip with its audio, the location when the observer started speaking, and the time. Clips are sent for transcription as they are recorded.
3. **Stop.** Pressing **Stop survey** writes a *Stop* record carrying the session's GPS track.

### Speaking an observation

Observations are marked with three command words. The defaults are shown here; they can be changed when the survey is created.

| Command word | Meaning |
|:--|:--|
| `observation` | Starts a new observation. Everything said until the stop word belongs to it. |
| `stop` | Ends the observation. If it is forgotten, the observation ends at the next command word or after about 15 seconds. |
| `correction` | Starts an observation that replaces the previous one. Say it, then the whole observation again. |

For example, with fill fields *Species*, *Count* and *Age class*:

> observation, species elephant, count four, age class adult, stop

Say the field name followed by its value. List items do not need the field name: the choice label on its own is enough, so "elephant" works as well as "species elephant". The example above could be said as:

> observation, elephant, count four, adult, stop

The fields are filled by an AI model that reads the whole observation for meaning, so the observer does not have to speak in a fixed order or a terse form. A rambling description such as "there are four elephants here, all adults, one of them is quite close to the road" still fills *Species*, *Count* and *Age class*. Command words are the only things that must be said exactly.

The screen lists every fill field and the values it accepts as a reminder of what can be said.

### From speech to events

Once every clip of a session has been transcribed, CyberTracker reconstructs the session as a single stream of words placed along the GPS track:

- The stream is split into observations at the command words.
- Each observation becomes one record, located where its first word was spoken.
- The spoken text is placed in the event's note, and an AI form-filler sets the fill fields from it.
- The audio that produced the observation is attached to the record. The raw clips are then deleted.

A record's status icon shows whether it is still transcribing, completed or submitted.

### Submitting

Records are never sent automatically. When transcription has finished, press **Submit** on the survey's start page. Each record is uploaded as an event of the chosen event type:

| Record | What EarthRanger receives |
|:--|:--|
| Start | An event at the start location, with the metadata fields. |
| Observation | An event at the observation location, with the metadata and fill fields, the transcript as the event note, and the audio as an event file. |
| Stop | An event at the stop location, with the GPS track as a CSV event file. |

The records are told apart by the *type field* (see below), which holds `Start`, `Data` or `Stop`. Submitted records are removed from the device.

The survey itself can be run offline: recording, GPS logging and the clips need nothing from the network. Transcription and form filling run in the cloud, so the device needs an internet connection afterwards before the records can be completed and submitted. Clips wait in a queue until they have been transcribed.

## Creating an event type for a talk survey

The talk survey uses the fields EarthRanger builds into every event: the location becomes the event geometry, the note receives the transcript, and the audio and track are uploaded as event files. The reporter is chosen from EarthRanger's *Reported by* list. None of these need to be added to the schema.

The event type itself needs the following fields. Create or edit the event type in EarthRanger and add them with the event type builder.

| Role | Field type in EarthRanger | Notes |
|:--|:--|:--|
| Type field | Text | Required. Receives `Start`, `Voice`, `Data` or `Stop`. For example, *Record type*. |
| Session id field | Text | Required. Receives an id shared by every record of one survey, so a survey can be reassembled in EarthRanger. For example, *Session*. |
| Metadata fields | Any | Optional. Entered once per survey on the start page and copied to every record. For example, *Transect* or *Team*. |
| Fill fields | Text, Numeric, Boolean, Single select, Multi select, Date, Time or Date time | At least one. Spoken in each observation and filled from the transcript. |

Use a **point** geometry for the event type. Each observation is a single location on the track.

### Tips for fields that transcribe well

- Field titles and choice labels are what the observer will say, and they are given to the transcriber as vocabulary. Keep them short, distinct and easy to pronounce.
- Avoid choice labels that sound alike, and choice labels that contain a command word.
- Numbers work best in Numeric fields. Yes/no questions work best as Boolean fields.
- The type and session id fields are managed by the app. Do not add constraints to them, such as a pattern or a minimum length, and do not reuse them for anything else.

## Creating the talk survey on the device

A talk survey is a *snapshot* of the EarthRanger connection: a separate project on the device holding just one event type, with its own pages.

1. Connect CyberTracker to EarthRanger and log in.
2. In the EarthRanger project, open **Settings** (the gear icon) and choose **Create snapshot**.
3. Choose **Talk survey**, then the event type.
4. On the setup page, assign the roles:
   - **Session id field**: the text field that receives the session id.
   - **Type field**: the text field that receives the record type.
   - **Metadata fields**: the fields entered once per survey.
   - **Fill fields**: the fields spoken in each observation. At least one is needed.
   - **Command words**: the start, stop and correction words. They must all differ.
5. Press the check mark. CyberTracker builds the package and installs it as a new project on the device.

The new project appears alongside the EarthRanger project. If the same talk survey already exists on the device, creating it again replaces it and deletes its data.

The talk survey needs the microphone and background location permissions, which it asks for the first time it runs.

## Running a survey

1. Open the talk survey project. On first use it asks you to log in and to choose who the events are reported by.
2. Press **New survey**, check the start location, enter the metadata fields and press **Start survey**.
3. Talk. The footer shows whether the recorder is listening or recording, and how many clips have been saved. The home button leaves the project with the survey still in progress; reopening the project returns to it.
4. Press **Stop survey** when done.
5. Back on the start page, wait for the records to finish transcribing, review them, then press **Submit**.

The **Map** button shows the records and the track. The settings page (gear icon) has login, the *Reported by* choice and an **Update** button that rebuilds the survey from the current event type on the server.
