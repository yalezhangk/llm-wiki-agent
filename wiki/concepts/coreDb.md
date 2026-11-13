---
title: "coreDb"
type: concept
tags: [coredb, database, easergy, rtu]
---

## Key Details
- coreDb is the real-time database at the center of Schneider Electric's Baseline Software Platform, around which all other elements are developed.
- It stores data points categorized into four tables: Status, Analog, Command, and Setpoint.
- A Point is a record in coreDb; a Device is a set of I/O points sharing a common source/destination, always associated with a Controller type.
- Sources define the origin of a point's value, while Destinations define the target; multiple sources/destinations are allowed for Command and Setpoint points but not recommended for Status and Analog.
- Coordinates uniquely identify points within a Device, with structure varying by Controller type.
- Configuration changes to coreDb are made via Easergy Builder plugins and transferred to the RTU as XML files, requiring a reboot to activate.
- MQTT Client Devices can map Status, Analog, and String points as sources or destinations, but do not support Command points.

## Related
- [[Easergy Builder]]
- [[MQTT]]
- [[T300]]
- [[Saitel DR]]

## Version Updates

- Rev 1.1 of the MQTT Client Device User Manual (dated 09/07/2025) confirms that MQTT Client Devices can map Status, Analog, and String points as sources or destinations, but do not support Command points, consistent with earlier documentation.
