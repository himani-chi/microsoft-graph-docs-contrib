---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc-beta communications calls answer post --call-id {call-id} --body '{\
  "callbackUri": "callbackUri-value",\
  "mediaConfig": {\
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",\
    "blob": "<Media Session Configuration Blob>"\
  },\
  "acceptedModalities": [\
    "audio"\
  ],\
  "callOptions": {\
    "@odata.type": "#microsoft.graph.incomingCallOptions",\
    "isContentSharingNotificationEnabled": true,\
    "isDeltaRosterEnabled": true,\
    "isInteractiveRosterEnabled": true\
  },\
  "participantCapacity": 200\
}\
'

```