# Wiki Log

Append-only chronological record of all operations.

Format: `## [YYYY-MM-DD] <operation> | <title>`

Parse recent entries: `grep "^## \[" wiki/log.md | tail -10`

---

## [2026-06-05] ingest | WSG-WIG 智能开关柜

Added source. Key claims: the 2019.2 Schneider Electric / SAS WSG-WIG smart switchgear deck frames online condition monitoring as part of substation automation and smart switchgear development. It cites NB/T 42044-2014 for 3.6kV-40.5kV intelligent AC metal-enclosed switchgear and controlgear, notes GB/T 2900.20-2016 terminology additions for intelligent switchgear, and states that intelligent components should be integrated with switchgear and tested with high-voltage switchgear under operating or simulated operating states. It records a WIG factory system diagram with gateway, optical switch, auxiliary monitoring backend, smart monitoring display terminal, Chengdu Jiaoda Yunda equipment, Changzhou Pasific equipment, Modbus-RTU, and a likely IEC61580/IEC61850 typo. It expands WSG/WIG monitoring scope to temperature monitoring of busbars and inner/outer cone cable heads, SF6 density and micro-water monitoring, partial discharge by pulse-current and TEV+ultrasonic methods, arc-light monitoring with overcurrent blocking and 5-7ms action claim, arrester resistive-current monitoring, three-position switch video, breaker mechanical characteristics, control-coil and charging-motor monitoring, I2t accumulation, and electrical-life monitoring. Project-plan, supplier, and price details are treated as 2019-stage context rather than current procurement facts.

## [2026-06-05] ingest | WS-G 40.5kV及以下气体绝缘开关柜 2014产品介绍

Added source. Key claims: the June 2014 Schneider Switchgear (Suzhou) WS-G presentation covers application scope, ratings, product structure, product advantages, five WS-G characteristics, wiring schemes, and operating examples. It positions WS-G for 12-40.5kV medium-voltage applications, standard altitude 1000m and special altitude 4000m, with applications in petrochemical, industry, infrastructure, power supply, metallurgy, marine, transport, and wind farms. Its historical rating set is 12/17.5/24/36/40.5kV, busbar and feeder natural-cooling current 2500A, short-time withstand 31.5kA/4s, peak withstand 80kA with higher values by consultation, and internal arc 31.5kA/1s. It documents sealed gas compartments, B-link without site SF6 handling, gas-density monitoring without gas piping, inner-cone and outer-cone cable-connection limits, low-voltage cabinet features, forced interlocking, single/double-busbar schemes, busbar auxiliary modules, environmental/recycling claims, and 2006-2014 Chinese operating examples across metro, petrochemical, salt-lake, coal-chemical, power-supply, and wind-grid mobile-substation projects.

## [2026-06-05] ingest | WS-G 气体绝缘金属封闭开关设备 操作说明书

Added source. Key claims: the WS-G operation instructions document `KSGA0.463.150-03` identifies WS-G as gas-insulated switchgear up to 40.5kV and covers service, overview, technical data/control and operating elements, schemes, insulating-gas monitoring, VDS, operation, switchgear operation, maintenance, appendices, and notes. The local PDF is truncated: its linearized header declares about 41.95MB while the available file is about 18.22MB, so only 31 scanned pages were recovered. From the recovered pages, the manual gives a conservative operation-manual rating set of 12/17.5/24/36/40.5kV, busbar/outgoing current <=2500A, short-circuit breaking current <=31.5kA, short-time withstand <=31.5kA/4s, and 50/60Hz; states that qualified personnel must perform operation and maintenance; describes optional electrical control elements; confirms SF6 sealed pressure-system gas tanks with no gas replenishment under normal service; documents standard IDIS with green/yellow/yellow-red status, remote signaling, and pressure thresholds; documents IVIS / plug-in VDS and first-energization phase checking; and describes manual operating panels plus mechanical interlocking to prevent incorrect operation.

## [2026-06-05] ingest | WS-G 12~40.5kV 交流金属封闭气体绝缘开关柜 产品目录

Added source. Key claims: the 2024.01 WS-G product catalog presents WS-G 12~40.5kV AC metal-enclosed gas-insulated switchgear for public and industrial distribution networks, infrastructure, mining, metallurgy, petrochemical, fuel/gas, railway power supply, container-base, and ship applications. It gives ratings up to 40.5kV, 3150A, 40kA breaking current, and IAC 40kA/1s; supports single-busbar and double-busbar systems; explains B-link busbar connection without on-site gas handling; lists gas-compartment pressure thresholds, VDS voltage detection, outer-cone/inner-cone cable-connection boundaries, low-voltage cabinet options, dimensions, weights, main wiring schemes, shipping documents, storage requirements, and ordering data. It reinforces the existing 3150A vs 4000A WS-G version/configuration distinction.

## [2026-06-05] ingest | WS-G 交流气体绝缘金属封闭开关设备 企业标准

Added source. Key claims: the Q/320500 KSGA 09-2015 enterprise standard defines WS-G/KGN23 as indoor AC gas-insulated metal-enclosed switchgear for 50Hz, 12kV-40.5kV single-busbar, double-busbar, or bus-section systems. It records ratings up to 4000A busbar current and 40kA short-time withstand, IP65 gas tanks, IP4X/IP5X/IK07 switchgear protection, LSC2A continuity, SF6 sealed pressure requirements with annual leakage rate <=0.1%, gas-density monitoring with low-pressure and minimum-function alarms, internal-arc AFL with optional AFLR, mandatory type-test items, routine factory tests, and WS-G/KGN23 model-code rules.

## [2026-06-05] ingest | WS-G 交流气体绝缘金属封闭开关设备 企业标准 2024

Added source. Key claims: Q/AVXM 031-2024 is a Schneider Electric (Xiamen) enterprise standard for WS-G indoor AC gas-insulated metal-enclosed switchgear, issued on 2024-07-01 and implemented on 2024-07-21. It keeps the 50Hz, 12kV-40.5kV single-busbar/double-busbar/bus-section scope, updates the reference-standard basis to GB/T 3906 and IEC 62271-200:2011, raises special-condition altitude to 5500m, records busbar and feeder currents up to 3150A, keeps IP65 gas tanks and LSC2A continuity, adds IDIS pressure-threshold notes, details cable-test and zero-gauge-pressure insulation tests, adds back-to-back capacitor-bank switching, and specifies high-altitude routine withstand-test parameters.

## [2026-06-05] ingest | WI-G 铁道用气体绝缘金属封闭开关设备 操作说明书

Added source. Key claims: the WI-G operation manual is a Schneider Electric operation-instructions document for gas-insulated switchgear for railway application. It confirms WI-G as a 31.5kV SF6-insulated metal-enclosed indoor railway switchgear with busbar/outgoing current up to 2500A, short-circuit breaking current up to 31.5kA, short-time withstand up to 31.5kA/4s, B-Link busbar connection, inner-cone cable connection, vacuum-interrupter circuit-breaker compartment, three-position switch busbar compartment, IDIS gas-density monitoring at 0.06MPa rated filling pressure with 0.05MPa pre-warning and 0.03MPa main warning, IVIS / plug-in VDS voltage detection, mechanical interlocking for safe operation, and a maintenance plan covering visual inspection, lubrication, partial-discharge checks, secondary-component checks, B-Link/plug inspection, and replacement after vacuum-interrupter limits or 10000 operating cycles.

## [2026-06-05] ingest | WS-G 40.5kV 气体绝缘开关柜图片页

Added source. Key claims: the JPG image presents WS-G 40.5kV gas-insulated switchgear for offshore-wind 35kV switchgear applications. It highlights GIS benefits for corrosion resistance, harsh operating environments, supply continuity, operator safety, and low maintenance, and gives ratings of 40.5kV, 95kV power-frequency withstand, 185kV lightning impulse withstand, 40kA/3s short-time withstand, 100kA peak withstand, 4000A double-busbar current, and IAC 40kA/1s. It also identifies B-LINK as a patented busbar connection technology and notes sealed gas compartments, per-compartment mechanical/electrical detection, independent pressure relief, and CrNi stainless-steel gas tanks.

## [2026-06-04] graph | Knowledge graph rebuilt

67 nodes, 433 edges (433 extracted, 0 inferred).


## [2026-06-04] ingest | GHA Gas-insulated Switchgear Catalog 2018

Added source. Key claims: the 2018 GHA catalog is the formal product catalog for gas-insulated switchgear up to 40.5kV, covering IEC single-busbar and double-busbar configurations, GHA Rail and GHA ANSI branches, general ratings of 12/17.5/24/36/38/40.5kV, 40kA short-time current, 100kA peak withstand current, busbar and branch currents up to 2500A with busbar values up to 4000A on request, IAC 40kA/1s, sealed pressure-system gas compartments according to IEC/EN 62271-1, B-link without site gas work, IDIS gas status LEDs and remote group warning, IVIS voltage detection, EcoStruxure-ready protection/metering/condition monitoring, TH110/CL110 monitoring, SF6 recovery, and 90% potential recyclability by weight. It refines the older PPT and flags a 100kA vs 104kA B-link peak-current wording difference.

## [2026-06-04] ingest | GHA Gas Insulated Switchgear Presentation Vers 06 English

Added source. Key claims: GHA is a Schneider Electric gas-insulated medium-voltage switchgear presentation from Regensburg, September 2010, positioned up to 40.5kV with vacuum circuit-breaker, single-busbar and double-busbar arrangements, B-link busbar connection without site gas handling, sealed pressure-system gas compartments with leakage rate <<0.1% p.a., IDIS gas-density indication per compartment, outer-cone cable connections up to 36kV, inner-cone connections up to 40.5kV, fully insulated busbar systems up to 2500A, ILIS internal-arc detection and turn-off around 100ms, IAC AFLR up to 40kA/1s, and seismic qualification options. Legacy PPT extraction fragmented some rating tables, so only clearly extracted values were recorded.

## [2026-06-04] ingest | WIG 高铁智能开关柜 交大运达保护 帕斯菲克视窗

Added source. Key claims: WIG is a high-speed-rail smart switchgear digital-substation integration deck dated 2018.4. It defines digital substations around fully digital information acquisition, transmission, processing, and output; uses an IEC 61850-style process/bay/station-layer architecture; and maps WIG factory-system equipment to gateways, merging intelligent units, protection and control devices, optical switches, auxiliary monitoring backends, protection-control backends, and smart monitoring display terminals. Monitored objects include breaker mechanical characteristics, spring-charging motor, three-position switch motor, arrester status, SF6 density and temperature, live indication, cabinet temperature, automatic heating/dehumidification, and reserved online detection. The deck identifies Chengdu Jiaoda Yunda, Changzhou Pasific, and Shenzhen Shengwei Electronic Technology supplier boundaries, and flags a likely IEC61580 vs IEC61850 typo in the protocol-conversion labels.

## [2026-06-04] ingest | PIX 户内交流金属封闭开关设备 产品目录 V8

Added source. Key claims: the V8 DOCX is a newer PIX Chinese catalog revision dated from the file metadata on 2024-06-12. It expands PIX to a 7.2/12/24kV comprehensive product-family view under GB/T 3906-2020 and IEC 62271-200:2021, gives IAC AFLR internal-arc ratings of 50kA/1s for 7.2/12kV and 40kA/1s for 24kV, keeps the 12kV generator-outlet branch up to 6300A and 63kA, updates cabinet-width and product-size tables, and adds Green Premium, PCCC, carbon-footprint certification, nuclear, marine, WMTS transfer, and Smart PIX digital-operation content tied to EcoStruxure, PMB/PMB Easy, Asset Advisor, wireless temperature monitoring, breaker characteristic monitoring, partial discharge, remaining electrical life, video, arc flash, and environmental monitoring.

## [2026-06-04] ingest | PIX 500 铠装式金属封闭开关设备 产品目录

Added source. Key claims: the file name contains PIX550, but the PDF body is PIX 500. PIX500 is a 500mm-width compact PIX-family 12kV air-insulated armored metal-enclosed switchgear branch using a fixed-connected main circuit, HVX embedded-pole vacuum circuit breaker, and a three-position switch with service/disconnect/earthing positions. It supports rated current up to 1250A and short-time withstand/breaking capability up to 31.5kA, offers front maintenance with a 1m front aisle, claims 30% civil-cost reduction versus traditional XGN substations, avoids SF6, and targets compact substations, tram, infrastructure, and other MV distribution scenarios.

## [2026-06-04] ingest | PIX550 中置式金属封闭开关设备 产品目录

Added source. Key claims: PIX550 is the smallest PIX-family 12kV center-mounted metal-enclosed switchgear branch for 50Hz single-busbar and bus-section systems. It uses a 550mm width, 2250mm height, 1400mm depth, supports rated current up to 1250A and short-time withstand/breaking capability up to 31.5kA, uses an HVX embedded-pole vacuum circuit-breaker truck, provides four compartments, five-prevention interlocks, pressure relief paths, front-maintenance options, wall/back-to-back/face-to-face installation, and can be directly coupled with PIX cabinets of other ratings and widths.

## [2026-06-04] ingest | PIX 户内交流金属封闭开关设备 产品目录

Added source. Key claims: the Chinese PIX catalog defines PIX as armored withdrawable indoor AC metal-enclosed switchgear and expands the PIX record with PIX-12kV, PIX-24kV, PIX-M contactor cubicles, and PIX-Gen generator-outlet breaker cubicles. PIX-12kV covers 630A-4000A and 20kA-50kA, PIX-Gen reaches 5000A/6300A and 63kA, PIX-24kV covers 630A-4000A and 20kA-40kA, and the catalog adds four functional compartments, five-prevention interlocks, pressure relief paths, HVX, VAH, CVX, ESW, MiCOM, primary scheme codes, ordering data, and installation requirements.

## [2026-06-04] ingest | PIX 50kA Catalogue EN

Added source. Key claims: PIX is a Schneider Electric air-insulated switchgear cataloged at 17.5kV, 50kA, and 4000A with HVX embedded pole; it uses LSC2B-PM metal-partitioned compartments, supports IAC AFLR 50kA/1s internal-arc classification, provides feeder, bus section, bus riser, busbar metering/earthing and contactor feeder functional units, and connects Easergy P3/P5, VAMP, TH110, CL110, SMD, HMI, SCADA/Services, cloud apps and mobile alarming into an EcoStruxure-ready operation chain.

## [2026-06-04] ingest | MVnex 中压金属铠装开关柜

Added source. Key claims: MVnex is a 12kV indoor metal-enclosed, withdrawable metal-clad switchgear family with standard, MVnex 550 compact, MVnex 500 ultra-compact, and Smart MVnex variants. The standard product reaches 4000A and 40kA, MVnex 550/500 target compact substations at 1250A and 31.5kA, HVX is the core vacuum circuit-breaker platform, and Smart MVnex combines TH110 temperature monitoring, Easergy P3, VAMP arc protection, active maintenance, and 千里眼.

## [2026-06-04] ingest | GMA Gas-insulated Switchgear Catalog 2017

Added source. Key claims: the English GMA catalog expands the international GMA parameter view to up to 24kV, 2500A, and 31.5kA, highlights compact 450mm feeders up to 800A, IAC AFL 1s as standard with AFLR optional, sealed pressure system behavior, no on-site gas handling, IoT / Smart Grid readiness, remote monitoring, and EcoStruxure-ready protection, metering, and condition-monitoring solutions. It also introduces a version/market-current-rating gap versus the Chinese 2023 GMA catalog.

## [2026-06-04] ingest | GMA Air C4C Digital Implement

Added source. Key claims: the single-slide deck is a digital implementation checklist for GMA Air / GM AirSeT, covering IED protection, metering and condition monitoring, CB electrical monitoring, gas density/temperature/humidity monitoring, RFID/Zigbee, TH110/TH110-R/CL110/SD20 sensor references, cable-side temperature rise monitoring, and partial discharge monitoring.

## [2026-06-04] ingest | GM AirSeT 中压一次气体绝缘开关柜 产品目录 V1.1

Added source. Key claims: GM AirSeT is an environmentally oriented 12kV metal-enclosed gas-insulated primary switchgear product that replaces SF6 with dry air / eco gas, keeps a GMA-like modular and plug-in architecture, supports IP67 sealed gas compartments, IAC AFLR 31.5kA/1s internal-arc performance, 31.5kA short-time withstand current, 2500m high-altitude testing, and avoids extra gas handling at installation, maintenance, and end of life.

## [2026-06-04] ingest | GMA 中压一次气体绝缘开关柜 产品目录 V1.5

Added source. Key claims: GMA is a 12/24kV SF6 gas-insulated, metal-enclosed, type-tested single-busbar primary switchgear product with modular expansion, plug-in installation, sealed pressure-system gas compartments, solid-insulated busbars, IAC 31.5kA/1s internal-arc testing, IP67 gas compartments, and functional units such as CB, BC, BR, DS, DI, PT, and metering cabinets.

## [2026-06-04] ingest | DNF7 户内交流金属封闭开关设备

Added source. Key claims: DNF7 is a 40.5kV indoor AC metal-enclosed switchgear product with LSC2B continuity, PM partitions, IAC AFLR 31.5kA/1s internal-arc classification, HVX-based functional units, and digital operation features including TH110 temperature monitoring, Smart HVX breaker characteristic monitoring, video monitoring, arc protection, remaining electrical-life monitoring, PMBox, PMB Easy, EcoStruxure, and asset-advisor connectivity.

## [2026-06-03] ingest | Smart HVX & PMBox 介绍

Added source. Key claims: the deck connects Smart HVX, PMB Easy, 千里眼, and PMBox in one active-maintenance narrative; it confirms PMB Easy single-unit/station-wide display roles and adds PMBox as an EcoStruxure Power edge-control product for asset management, state monitoring, predictive maintenance, 3D station views, partial-discharge analysis, and historical data queries.

## [2026-06-03] lint | Wiki health check

Ran wiki-lint using local structural checks and agent semantic review. Found four source-page orphans, no broken wikilinks, no missing entity pages, and one reliability-metric wording inconsistency to keep tracking.

## [2026-06-03] ingest | Smart HVX 智能中压断路器 产品简介

Added source. Key claims: Smart HVX builds on HVX and offers basic temperature, standard temperature, and intelligent configurations; PMB Easy serves as the proactive maintenance unit; the brochure emphasizes temperature monitoring, switchgear-state monitoring, and secondary-component monitoring as the core differentiators.

## [2026-06-03] lint | Wiki health check

Ran structural lint successfully and reviewed semantic issues manually because local litellm provider/model configuration is unavailable. Found one orphan concept page and a broader Chinese text encoding readability issue in multiple wiki files.

## [2026-06-03] ingest | Smart HVX 智能中压断路器 方案总览

Added source. Key claims: the one-page overview confirms the three Smart HVX configuration tiers, clarifies local and cloud display paths, and makes the topology around PMB Easy, 千里眼, ZBRN32, Link150, and BMM more explicit.

## [2026-06-03] ingest | HVX 中压真空断路器系列 说明书

Added source. Key claims: the HVX manual clarifies the base breaker platform across 12kV, 24kV, and 40.5kV classes, documents design features such as vacuum interrupters and solid-sealed poles, and adds detailed secondary-device, selection, and ordering information.

## [2026-06-03] ingest | PMB Easy 主动运维智能单元 产品简介

Added source. Key claims: the PMB Easy brochure turns PMB Easy into a standalone device record by clarifying single-unit versus station-wide deployment, supported monitoring objects, topology roles alongside ZBRN32/Link150/BMM, and concrete hardware model and installation parameters.

## [2026-06-03] ingest | PMB Easy 主动运维智能单元 演示稿

Added source. Key claims: the PPT deck largely corroborates the PMB Easy brochure, confirming single-unit versus station-wide deployment, supported monitoring objects, topology roles with ZBRN32/Link150/BMM, and the cabinet-door installation recommendation.

## [2026-06-03] ingest | Smart HVX 产品介绍 V3.4

Added source. Key claims: the V3.4 product deck expands Smart HVX's sales and application narrative with temperature-technology comparisons, reliability commitments, maintenance-efficiency rationale, 千里眼 labor-saving examples, and typical distribution-room topology. It also flags a reliability-metric wording inconsistency for later verification.
