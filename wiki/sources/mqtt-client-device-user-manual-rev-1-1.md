---
title: "MQTT Client Device User Manual Rev 1.1"
type: source
tags: [mqtt, easergy-builder, t300, communication, schneider-electric]
date: 2025-07-09
source_file: raw/uploads/manual/MQTT---User-Manual-_EN_1.1.pdf
---
## Summary
This manual (SE-MQTT-S854, Rev 1.1, dated 09/07/2025) provides configuration instructions for the MQTT Client Device plugin within the Easergy Builder tool. It updates the software version requirements to Easergy Builder 01.07.49 and MQTT Client Plugin 01.00.05. The document details the Baseline Software Platform architecture, coreDb integration, hardware compatibility for Saitel DR and PowerLogic T300 platforms, and MQTT protocol specifics including broker connection parameters (QoS, TLS, Sparkplug) and topic mapping.

## Key Claims
- The MQTT Client Device is a plugin for Easergy Builder, supporting software versions 01.07.49 (Easergy Builder) and 01.00.05 (MQTT Client Plugin).
- Hardware compatibility is limited to Saitel DR platforms (HU_B/HU_BI, HU_A/HU_AF, HUe) and PowerLogic T300 (HU250); Saitel DP platforms (SM_CPU866, SM_CPU866e) do not support the MQTT Client.
- The Baseline Software Platform consists of VxWorks & Linux operating systems, real-time applications, and configuration tools, with coreDb as the central real-time database.
- coreDb points are categorized into Status, Analog, Command, and Setpoint tables; MQTT devices can map Status, Analog, and String points as sources or destinations, but Command points are not supported.
- MQTT coordinates follow the format `[TOPIC ID] [POINT NAME]`, where the Topic ID is defined in the device configuration and the Point Name identifies the specific data point.
- The MQTT broker connection configuration includes parameters for ID, QoS (At most once, At least once, Exactly once), MQTT Version (3.1.1 or 5), URL (IPv4/IPv6), Interval (min 50ms), TLS encryption, Port, and Sparkplug specification.
- Topics are defined with Value, ID, and Format (XML or JSON), and subscription/publication is configured in coreDb rather than directly in the topic definition.
- The manual emphasizes that configuration changes in Easergy Builder are transferred to the RTU via XML files and require a reboot to take effect.

## Connections
- [[Easergy Builder]] — configuration tool for the MQTT Client Device.
- [[T300]] — PowerLogic T300 platform supporting the MQTT Client.
- [[Saitel DR]] — Saitel DR head units (HU_B, HU_A, HUe) supporting the MQTT Client.
- [[MQTT]] — communication protocol used by the client device.
- [[coreDb]] — real-time database central to the Baseline Software Platform.
- [[Schneider Electric]] — manufacturer of the software and hardware platforms.

## Contradictions
- The software versions listed in this Rev 1.1 manual (Easergy Builder 01.07.49, MQTT Plugin 01.00.05) differ from the Rev 1.0 manual (Easergy Builder 01.07.45, MQTT Plugin 01.00.02). This is a version update, not a contradiction, but the newer versions should be used for current configurations.