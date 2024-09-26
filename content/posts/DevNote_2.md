---
title: "Development Note #2"
summary: "Fix stuttering issue with Unreal Engine 5.4, as of July 2024."
date: 2024-07-24T22:43:50-05:00
tags:
  - dev note
  - unreal engine
author: "a_nightails"
---
## Introduction 👋
Welcome to my second development note. This one is focusing on a particular issue that I have with Unreal Engine 5.4 on
Linux, and possibly Windows due to telemetry.

## Note 📝
Currently, UE5.4 editor will be stuttering on start-up and possibly crash.

To fix this, **DISABLE** the `StudioTelemetry`plugin.

Add this part to the `*.uproject` if the editor is too lagged and unresponsive:

`{ "Name": "StudioTelemetry", "Enabled": false }`
