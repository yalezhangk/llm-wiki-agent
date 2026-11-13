---
title: "MQTT"
type: concept
tags: [mqtt, communication, protocol, iot]
---

## Key Details
- MQTT (Message Queuing Telemetry Transport) operates on a publish/subscribe model, decoupling message senders (publishers) from receivers (subscribers) via a message broker.
- The broker handles space, time, and synchronization decoupling, allowing publishers and subscribers to operate independently of each other's network location and timing.
- An MQTT client is any device running an MQTT library, acting as a publisher when sending messages and a subscriber when receiving them.
- The MQTT broker is responsible for authorizing/authenticating clients, filtering messages, and handling missed messages and client sessions.
- Clients connect to the broker via TCP/IP using CONNECT and CONNACK messages; clients never connect directly to each other.
- In the context of Schneider Electric's Baseline Software Platform, the MQTT Client Device plugin allows RTUs to publish coreDb data points to topics and subscribe to external topics for data ingestion.
- Supported MQTT versions include 3.1.1 and 5, with configurable QoS levels (At most once, At least once, Exactly once) and optional TLS encryption.
- Sparkplug specification support is available for standardized industrial telemetry data exchange.

## Related
- [[Easergy Builder]]
- [[coreDb]]
- [[T300]]
- [[Saitel DR]]

## Version Updates

- Rev 1.1 of the MQTT Client Device User Manual (dated 09/07/2025) updates the supported software versions to Easergy Builder 01.07.49 and MQTT Client Plugin 01.00.05, replacing the earlier 01.07.45/01.00.02 versions.
