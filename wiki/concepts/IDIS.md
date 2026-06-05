---
title: "IDIS"
type: concept
tags: [gas-monitoring, gas-insulated-switchgear]
sources: [gha-gas-insulated-switchgear-presentation-vers-06-englisch, gha-nrjcat18789en-0318, qavxm-031-2024-wsg-enterprise-standard, wi-g-railway-gas-insulated-switchgear-operation-instructions, wsg-gas-insulated-metal-enclosed-switchgear-operation-instructions]
last_updated: 2026-06-05
---

## Summary
[[IDIS]] is the gas-density / gas-status information system described for [[GHA]], [[WSG]] and [[WIG]]. It turns [[气室监测]] into a visual and remote-signaling function by combining compartment sensors or density switches with a traffic-light display and remote warning contacts.

## Key Details
- IDIS is presented as a gas-density information system rather than a generic pressure gauge.
- Each gas-filled compartment is autonomous and monitored separately.
- The older presentation describes a temperature-compensated gas density switch; the 2018 catalog describes a pressure sensor whose electrical signals are retransmitted to the IDIS display.
- The indication supports green OK, yellow pre-warning, and red main-warning levels.
- The system avoids gas pipes within a panel or between panels.
- The display uses green/yellow/red visual indicators for compartment status.
- The catalog states that any warning level can be signalled remotely as a common gas warning group signal for the whole switchgear.
- The WS-G 2024 enterprise standard adds IDIS pressure-threshold notes for low-pressure alarm and minimum functional pressure.
- The WI-G operation manual describes a temperature-compensated IDIS system whose LED signals come from up to three gas-density switches.
- WI-G routes IDIS signals through communication wiring to remote-control or I&C systems.
- WI-G uses green for ready for operation, yellow for pressure-drop pre-warning, and red for pressure-drop main warning.
- WI-G gives IDIS reference values at 31.5kV: rated filling pressure 0.06MPa, pre-warning 0.05MPa, and main warning 0.03MPa.
- The WS-G operation manual states that each panel is equipped with IDIS as standard for insulating-gas monitoring.
- The WS-G manual describes IDIS as a temperature-compensated gas-density information system that sends up to three gas-density switch signals through colored LEDs.
- The WS-G manual states that IDIS can pass signals to remote-control or I&C systems through communication relays on the rear side.
- The WS-G manual uses green for ready for operation, yellow for pressure-drop pre-warning, and yellow/red for pressure-drop main warning.
- WS-G pressure references in the manual are 0.03/0.015/0.01MPa for 12/24kV up to 1250A, 0.05/0.03/0.01MPa for 12/24kV above 1250A, 0.05/0.03/0.01MPa for 36kV, and 0.06/0.05/0.03MPa for 40.5kV.

## Related
- [[GHA]]
- [[WSG]]
- [[WIG]]
- [[IVIS]]
- [[气室监测]]
- [[气体绝缘开关柜]]
- [[数字化中压运维]]
