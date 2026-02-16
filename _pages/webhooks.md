---
layout: home
title: Webhooks
permalink: /webhooks/
nav_order: 7500
---
# Webhooks

CyberTracker supports **webhooks** that allows collected data to be automatically sent to a URL as JSON in a uniform format. This enables integration with custom backends. This works across all supported subsystems, including CyberTracker Online, CyberTracker Classic, SMART, EarthRanger, KoBoToolbox, ODK, Survey123 and Google Forms.

## Setup
Configuring a webhook in CyberTracker can be done in three ways:

### 1. Manual Configuration in the App
1. Open **CyberTracker**
2. Go to the **Settings** screen
3. Under the **Archive** option, tap **Webhook**
4. Enter the webhook URL manually in the text field

### 2. Applink
Create an applink which will configure CyberTracker with the webhook. This is useful for remote deployments or in cases where copy and pasting is not desirable.

The applink format is: `https://cybertrackerwiki.org/applink?x=<base64-encoded-json>`

Where `<base64-encoded-json>` is:

```json
{
  "webhook": true,
  "url": "https://mysite.com/webhook",
  "entity": "My entity"
}
````

The above json therefore becomes: `https://cybertrackerwiki.org/applink?x=ewogICJ3ZWJob29rIjogdHJ1ZSwKICAidXJsIjogImh0dHBzOi8vbXlzaXRlLmNvbS93ZWJob29rIiwKICAiZW50aXR5IjogIk15IGVudGl0eSIKfQ==`

When the link is opened on a device with CyberTracker installed, the app will prompt the user to confirm installation of the webhook for `My entity`. Note that if CyberTracker is not yet installed, then the user will be pointed to a web page with a link to it.

### 3. QR Code
Converting the above applink to a QR code and scanning it with CyberTracker is also supported.

## Payload format
When an observation is saved or sent, CyberTracker will **POST** a JSON object to the configured webhook URL.

### Single record payload

```json
{
  "uid": "b9b1c075e002441db6ada01225fb0a6f",
  "createTime": "2025-06-17T23:00:33.999+01:00",
  "updateTime": "2025-06-17T23:00:33.999+01:00",
  "sessionId": "15c17035a9514feebd48097e056c0211",
  "deviceId": "42dc6a06650b4e4a889faf9819b88e4a",
  "summary": "Test, This is a note",
  "username": "Justin",
  "location": [11.394516667, -0.310066667, 0, 1],

  "project": {
    "connector": "Classic",
    "provider": "Classic",
    "reportedBy": "",
    "subtitle": "Sample",
    "title": "Photo notes",
    "uid": "CLASSIC2_3bf5cf553eda4776af8b9f5c88c6134e"
  },

  "records": [
    {
      "summary": "Test, This is a note",
      "uid": "b9b1c075e002441db6ada01225fb0a6f",
      "values": [
        { "id": "Name", "name": "Name", "value": "Test" },
        { "id": "Photo", "name": "Photo", "value": null }, 
        { "id": "Note", "name": "Note", "value": "This is a note" },
        { "id": "Sound", "name": "Sound", "value": null }
      ]
    }
  ]
}
```

### Multi-record payload

SMART has a more complex format where the metadata is in the first record. The "IncidentRecord" field links to the other records. The GroupList and SMART_SightingGroupId field enable grouping of records when the `Use group UI` feature is enabled in SMART Desktop.

```json
{
  "uid": "1da3eb5fb71c42c29ecd547324541589",
  "createTime": "2025-06-17T23:41:54.760+01:00",
  "updateTime": "2025-06-17T23:41:54.764+01:00",
  "sessionId": "9b4d58911b0f40f185944276071e6b8b",
  "deviceId": "42dc6a06650b4e4a889faf9819b88e4a",
  "summary": "Independent Incident, None, PRIMATES, 3, Observed Only, Fig, Ripe",
  "username": "Justin",
  "location": [11.4382, -0.43205, 0, 1],

  "project": {
    "connector": "SMART",
    "provider": "SMART",
    "reportedBy": "",
    "subtitle": "2025/06/10 18:38:05",
    "title": "Conservation area sample",
    "uid": "SMART_9132eede-f804-483e-b686-9f063138b69a"
  },

  "records": [
    {
      "summary": "0.432050° S, 11.438200° E, Independent Incident",
      "uid": "1da3eb5fb71c42c29ecd547324541589",
      "values": [
        { "id": "GroupList", "name": "GroupList", "value": ["3ee253493c9243e89d2f4d822b9e2af2"] },
        { "id": "Location", "name": "Location", "value": [11.4382, -0.43205, 0, 1] },
        { "id": "SMART_ObservationType", "name": "SMART_ObservationType", "value": "Observation" },
        { "id": "SMART_DataType", "name": "Data Type", "value": "incident" },
        { "id": "SMART_IncidentType", "name": "Incident type", "value": "Independent Incident" },
        { "id": "SMART_Employees", "name": "Employees", "value": ["John Peter", "Lilian Wendy", "Samnang Tang"] },
        { "id": "IncidentRecord", "name": "Records", "value": ["7cd1ca59fee64899a0cfcc5b4c1b2dcd", "4ca8bd3d8fe24be3a680a8f8bfd2286e"] }
      ]
    },
    {
      "summary": "None, PRIMATES, 3, Observed Only",
      "uid": "7cd1ca59fee64899a0cfcc5b4c1b2dcd",
      "values": [
        { "id": "SMART_SightingGroupId", "name": "SMART_SightingGroupId", "value": "3ee253493c9243e89d2f4d822b9e2af2" },
        { "id": "a:0:a6e5c90fc4bb4e55890ae1656d7f4f67", "name": "Threat", "value": "None" },
        { "id": "a:0:2389593093a14c83855d50771f175f2b", "name": "Species", "value": "PRIMATES" },
        { "id": "a:0:9fa038f8287c48edbaa01ca8a0665d81", "name": "Number of Adult Males", "value": 3 },
        { "id": "a:0:309a27eedea9439d8af0437d4de375cf", "name": "Action Taken Live Animals", "value": "Observed Only" }
      ]
    },
    {
      "summary": "Fig, Ripe",
      "uid": "4ca8bd3d8fe24be3a680a8f8bfd2286e",
      "values": [
        {"id": "SMART_SightingGroupId", "name": "SMART_SightingGroupId", "value": "3ee253493c9243e89d2f4d822b9e2af2" },
        {"id": "a:0:90cd57d395ae49fea10e2757be45b9c8", "name": "Fruit or Nut Tree Species", "value": "Fig" },
        {"id": "a:0:d0c716cf9aee4b0f9391426b8c0d0e29", "name": "Fruiting Status", "value": "Ripe" }
      ]
    }
  ]
}
```

### Field descriptions

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>createTime</td>
      <td>ISO 8601 timestamp for when the data was created</td>
    </tr>
    <tr>
      <td>updateTime</td>
      <td>ISO 8601 timestamp for when the data was last updated</td>
    </tr>
    <tr>
      <td>deviceId</td>
      <td>Unique identifier for the device – created at install time, i.e. not unique across installs</td>
    </tr>
    <tr>
      <td>location</td>
      <td>JSON array containing [longitude, latitude, altitude, accuracy]</td>
    </tr>
    <tr>
      <td>project</td>
      <td>Metadata about the form project</td>
    </tr>
    <tr>
      <td>sessionId</td>
      <td>Unique identifier for the session. For SMART this is also the patrol id.</td>
    </tr>
    <tr>
      <td>uid</td>
      <td>Unique identifier for this observation. This may be repeated if the data is edited and resent. Always equivalent to the first records `uid` field</td>
    </tr>
    <tr>
      <td>username</td>
      <td>User specified in the 'Collect as' field on the Settings page</td>
    </tr>
    <tr>
      <td>summary</td>
      <td>The summary is typically a concatenation of field values, but is customizable by the project</td>
    </tr>
    <tr>
      <td>records</td>
      <td>List of records collected in the session - see below</td>
    </tr>
  </tbody>
</table>

### 'records' description
Each record contains a list of fields and their associated values. Irrelevant and undefined field values are not included.

Records may contain links to sub-records. In this case, the value will be an array of record `uid` values. This makes it possible to reconstruct a tree of data from the flattened records. Alternatively, if the data is modelled relationally, then each record can be mapped to a single table.

---

## Best Practices

* Use HTTPS for your webhook URLs to ensure secure transmission
* Respond to webhook POST requests with `HTTP 200 OK` to acknowledge receipt
* `uid` may be duplicated across different payloads in cases where records are edited and resent
