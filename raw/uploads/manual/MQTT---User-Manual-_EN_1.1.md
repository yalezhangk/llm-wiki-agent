Baseline Software Platform

MQTT Client Device

User Manual

This manual provides information about the configuration of the MQTT client device in
Easergy Builder.

SE-MQTT-S854

Publication Date (04/2025)

Read carefully the information contained in this manual before use this software tool for configuring the
control system.

www.se.com

16/04/2025

User Manual – MQTT Device

Change Control

Rev  Date

Description

1.0

16-04-2025

Initial revision for Easergy Builder.

1.1

09/07/2025  MQTT sensitive data update

General Information

The Baseline Software Platform and all its components have been developed in accordance to the
requirements for a quality management system, complying with the ISO 9001:2015 Norm.

Document code:

SE-MQTT-S854

Revision/Date:

1.0 / 16-04-2021

File:

MQTT – User Manual_EN_1.0.pdf

Retention period:

Permanent throughout its validation period + 3 years after its cancellation.

Reference Documents

Table 1 – Reference Documents

User Manual

webApp User Manual

Document Code

FTE-WPP-S856

Easergy Builder – User Manual

SE-MSS-USR

T300 User Manual

T300 Quick Start Guide

NT00378

NT00383

Software in Easergy Builder

The information contained in this document is applicable to the following software versions:

Table 2 – Software versions

Main Software / Plugin

Version (T300)

Easergy Builder Tool

MQTT client Device (Plugin)

01.07.49

01.00.05

Hardware/Software Compatibility

Controllers and software tools supported by each type of CPU is detailed are the following:

Table 3 – Hardware / Software compatibility

Pag 2

User Manual – MQTT Device

Platform

Saitel DP

Saitel DP

Saitel DR

Saitel DR

Saitel DR

16/04/2025

PowerLogic
T300

Tool / Software

SM_CPU866

SM_CPU866e  HU_B/HU_BI

HU_A/HU_AF  HUe

HU250

Easergy Builder

MQTT Client

webApp

√

×

×

√

×

√

√

×

×

√

×

×

√

×

√

√

√

√

Important information about Safety

Read these instructions carefully and look at the equipment to become familiar with it before trying
to install, operate, service or maintain it. In this manual can be found different types of messages
associated with situations that have different level of risk for people and / or for equipment.

This symbol indicates 'DANGER' or 'WARNING'. This symbol informs of an electrical
risk that will cause personal injuries if the instructions are not followed.

This symbol is associated to a safety alert. It is used to warn of possible personal
injury hazards. The user must follow all instructions or messages associated to this
symbol to avoid possible injuries.

DANGER indicates a hazardous situation which, if not avoided, will result in death or serious
injury.

DANGER

WARNING indicates a hazardous situation which, if not avoided, could result in death or
serious injury.

  WARNING

NOTICE is used to address practices not related to physical injury. The safety alert symbol shall
not be used with this signal word.

NOTICE

To Keep in Mind

Electrical equipment should be installed, operated, serviced, and maintained only by qualified
personnel. No responsibility is assumed by Schneider Electric for any consequences arising out of
the use of this material.

Qualified personnel are individuals who:

•  Have read and understood the information on the device and its user manual.

•  Are familiar with the installation, commissioning, and operation of the equipment and of the

system to which it is being connected.

Pag 3

16/04/2025

User Manual – MQTT Device

•  Are able to safely perform switching operations in accordance with accepted safety

engineering practices and are authorized to energize and de-energize equipment and to
isolate, ground, and label it.

•  Are trained in the care and use of safety apparatus in accordance with safety engineering

practices.

•  Are trained in emergency procedures (first aid).

It is necessary to consider that the documentation of the equipment collects the instructions for its
installation, set up and operation. However, the manuals could not cover all the possible
circumstances neither include specific information on all the details.

In case of questions or specific problems about a Schneider Electric’s equipment, contact with his
sales office of Schneider Electric or with the customer care center and request the necessary
information.

Symbols and Labels

Before the equipment is installed or commissioned, the user must understand the following
symbols, which may be used on the equipment or referred to in the user documentation:

Table 4 – Symbols

Symbol

Associated Text

Description

Possibility of electric
shock

International Electrotechnical Commission (IEC)
symbol associated to a DANGER or WARNING
message indicating that there is an electrical risk.
Failure to follow these instructions could cause
damage to people or death.

Caution, read the manual.

Symbol associated with a risk alert. The user must
read the manual before handling the equipment.

Possibility of electric
chock

Protective earth
connection

Functional earth
connection

CE Mark

Electronic equipment.
Special instructions must
be followed for disposed.

Compliant with RoHS.

Direct Voltage

Alternate Voltage

American National Standards Institute (ANSI) symbol
associated to a DANGER or WARNING message
indicating that there is an electrical risk. Failure to
follow these instructions could cause damage to
people or death.

Associated symbol to the protective ground
connection.

Associated symbol to the functional ground
connection.

This symbol indicates that the equipment has been
developed in compliance with all applicable
European Directives.

This symbol indicates that, at the end of its life, this
module must be disposed according to the WEEE
Directive (Waste Electrical and Electronic
Equipment).

The equipment has been designed and
manufactured according to RoHS Directive
(Restriction of Hazardous Substances).

Symbol of direct voltage (VDC).

Symbol of alternate voltage (VAC).

Pag 4

User Manual – MQTT Device

16/04/2025

Installation, Setup and Operation

Some devices use dangerous voltages (> 50 V), either the Schneider Electric device itself or some
device connected to it. The user is responsible to check that the characteristics of each equipment
are adapted and convenient for any installation. The user should read the instructions of installation
before proceeding to the use or maintenance of the equipment.

Not following these instructions can be dangerous for the people and the equipment.

  DANGER

Devices that handle dangerous tensions are marked with a sticker on the front label (size: 12,5
mm). This label must be visible all the time while the module is installed on the DIN rail.

Because of the variety of uses of the product, the managers of the application and use of this
controller device will have to take the measures to the fulfillment of all the safety requirements and
provision of each application. These requirements are according to the applicable laws,
regulations, codes and standard.

Pag 5

16/04/2025

Contents

1

2

User Manual – MQTT Device

EASERGY BUILDER & MQTT ................................................................................. 7

MQTT CLIENT ....................................................................................................... 15

Pag 6

1  Easergy Builder & MQTT

16/04/2025

Contents

User Manual – MQTT Device

1

EASERGY BUILDER & MQTT ................................................................................. 7

1.1.1

1.1  SOFTWARE ARCHITECTURE .................................................................................... 9
INTRODUCTION ............................................................................................... 9
1.2  EASERGY BUILDER ............................................................................................... 11
1.2.1  ENVIRONMENT DESCRIPTION ......................................................................... 11
1.2.2  DEVICE CATALOG ......................................................................................... 12
INTRODUCTION TO THE MQTT PROTOCOL ............................................................. 13
1.3.1  MQTT CLIENT .............................................................................................. 13
1.3.2  MQTT BROKER ............................................................................................. 13
1.3.3  MQTT CONNECTION...................................................................................... 14

1.3

Pag 8

User Manual – MQTT Device

16/04/2025

1.1  Software Architecture

1.1.1

Introduction

The Baseline Software Platform of Schneider Electric is composed by:

•  VxWorks & Linux operating systems.

•  Real-time applications and its configuration files.

•  Configuration, management, supervision and monitorization tools.

NOTICE

Saitel DR’s basic head units HU_B and HU_BI modules do not run VxWorks nor Linux. They
operate with a tailored-made OS which includes the database and applications.

Figure 1  – Baseline Software Platform

The operating system abstracts the hardware from the software applications and manages the
applications in real time. It integrates the basic protocols to access the remote unit (SFTP, SSH,
etc.) and manage multiple users.

The real-time database, named coreDb, is probably the most important element. All the other
elements are developed around coreDb.

Figure 2  – Relation between coreDb and other applications.

Pag 9

16/04/2025

User Manual – MQTT Device

The following concepts are related to coreDb:

•  Device Controller (also referred to as Controller): Real-time application that accesses
coreDb. Each Controller acts as a producer and/or consumer of information managed by
coreDb.

•  Point: Each record of coreDb is a point. A point can be included in the table Status, Analog,

Command or Setpoint.

•  Device:  A set of I/O points that share a common source/destination. A typical example of a

Device is an IED that communicates with the RTU, or the representation of a SCADA
exchanging information acquired or generated by the RTU. A Device is always associated to a
type of Controller.

•  Source: Origin of the value of a coreDb data point. Any coreDb data point can have several

different sources (in one or several Devices). This means that a value of a database point can
be configured to be updated by several different entities.

Note that any coreDb signal can be associated to more than one source; this is only applicable
to Command and Setpoint tables. Allocating more than source to one point is not
recommended in Status and Analog tables.

  WARNING

•  Destination: Target of the value of a coreDb data point. coreDb data points can be configured

to have several different destinations (in one or several Devices).

•  Coordinate: Point identification within a Device. It is unique for each point and has a different

structure for each Controller. It is described in detail in the appropriate manual of each
Controller.

•  Configuration Plugin: Specific Configuration plugins extend the Easergy Builder application to

configure Device Controllers. Additional details about these plugins are provided in their
manuals.

The user can modify the configuration of each Controller and Device using the appropriate Plugin.
Once the database is completely configured, the files with the new information can be generated
and transferred to the RTU, where they will be processed by the software on startup.

NOTICE

The configuration information exchanged between the RTU and Easergy Builder is not
continuous but performed through XML files under user’s request. When the configuration is
modified in Easergy Builder and the XML files are sent to the RTU, it is necessary to
reboot the RTU.

Pag 10

User Manual – MQTT Device

16/04/2025

1.2  Easergy Builder

1.2.1

Environment Description

The access to Easergy Builder is done through the Windows® Home Menu, or through the direct
access created on the desktop:

Figure 3  – Startup window of Easergy Builder.

The Easergy Builder tool starts on Workspace mode, where it is possible to administrate all the
RTUs and Configurations:

Figure 4  – Easergy Builder on WorkSpace mode.

On the Easergy Builder's WorkSpace mode there are four different areas:

•  1: Main menu

•  2: Administration toolbar

Pag 11

16/04/2025

User Manual – MQTT Device

•  3: RTU tree

•  4: Edition area

•  5: Consoles information

In the RTU tree, double click on the Configuration to be modified and the Configuration mode will
be shown in a new window:

Figure 5  – Configuration mode.

On the Configuration mode, the following areas are available:

•  1: Main menu

•  2: Section menu: Type of information to be shown on the editing zone. Devices, Channels,

coreDb and Synchronization are available.

•  3: Edition zone

•  4: Console view

•  5: Devices catalog

1.2.2

Device Catalog

The Device Catalog is a library where Device templates are stored. The user can create new
templates (stored in the PC) or re-use them to create new Devices in several Configurations and
RTUs.

A new template can be created by right-clicking on a Device on the Device tree and selecting
'Create template'. A name is requested for the new template, and it is generated with the same
structure and settings as the Device used.

Available templates are shown in the Device catalog.

Pag 12

User Manual – MQTT Device

16/04/2025

Figure 6  – Device catalog.

1.3  Introduction to the MQTT Protocol

It is highly recommended that the user be familiar with the MQTT specification prior to
configuring the RTU.

NOTICE

The MQTT protocol works on the principles of the publish/subscribe model. In traditional network
communication, clients and servers communicate with each other directly. The clients request
resources or data from the server, then the server processes and sends back a response.
However, MQTT uses a publish/subscribe pattern to decouple the message sender (publisher)
from the message receiver (subscriber). Instead, a third component, called a message broker,
handles the communication between publishers and subscribers. The broker’s job is to filter all
incoming messages from publishers and distribute them correctly to subscribers. The broker
decouples the publishers and subscribers as below:

•  Space decoupling: The publisher and subscriber are not aware of each other’s network

location and do not exchange information such as IP addresses or port numbers.

•  Time decoupling: The publisher and subscriber don’t run or have network connectivity at

the same time.

•  Synchronization decoupling: Both publishers and subscribers can send or receive

messages without interrupting each other. For example, the subscriber does not have to
wait for the publisher to send a message.

1.3.1   MQTT Client

An MQTT client is any device from a server to a microcontroller that runs an MQTT library. If the
client is sending messages, it acts as a publisher, and if it is receiving messages, it acts as a
receiver. Basically, any device that communicates using MQTT over a network can be called an
MQTT client device.

1.3.2   MQTT broker

The MQTT broker is the backend system which coordinates messages between the different
clients. Responsibilities of the broker include receiving and filtering messages, identifying clients
subscribed to each message, and sending them the messages. It is also responsible for other
tasks such as:

Pag 13

16/04/2025

User Manual – MQTT Device

•  Authorizing and authenticating MQTT clients.

•  Passing messages to other systems for further analysis.

•  Handling missed messages and client sessions.

1.3.3   MQTT connection

Clients and brokers begin communicating by using an MQTT connection. Clients initiate the
connection by sending a CONNECT message to the MQTT broker. The broker confirms that a
connection has been established by responding with a CONNACK message. Both the MQTT client
and the broker require a TCP/IP stack to communicate. Clients never connect with each other, only
with the broker.

Pag 14

2  MQTT Client

16/04/2025

Contents

User Manual – MQTT Device

2

MQTT CLIENT ....................................................................................................... 15

2.1  MQTT CLIENT ADMINISTRATION ........................................................................... 17
2.1.1  SIGNAL IDENTIFICATION - COORDINATES ........................................................ 17
2.1.2  RELATIONSHIP WITH COREDB ........................................................................ 17
2.2  MQTT CLIENT IN EASERGY BUILDER .................................................................... 18
2.2.1  DEVICE CONFIGURATION ............................................................................... 19

Pag 16

User Manual – MQTT Device

16/04/2025

2.1  MQTT Client Administration

2.1.1

Signal Identification - Coordinates
The coordinates of the points for the MQTT client device have the following format:

MQTT client coordinate

[TOPIC ID] [POINT NAME]

Where:

•  TOPIC ID: Name of the topic defined in the configuration of the device.

•  POINT NAME: Identifier of the point inside the topic. If the coordinate is defined as a

destination, the device will publish a point to the topic ID with the point name. If the coordinate
is defined as an origin, the device will read from the point name inside the topic ID.

Example: ‘t1 configFail’.

2.1.2

Relationship with coreDb

Possible Mappings

Once the coordinate’s format is defined, the user needs to determine the point types (according to
the coreDb) and the mode (source or destination) allowed for coordinates.

Status, Analog and String points can be mapped as source or destination. Command points are not
supported as mapping for MQTT devices.

When a point is configured as a destination, its value will be published periodically.

When a point is configured as a source, the client will subscribe to the corresponding topic and
update the value in CoreDB according to the value of that topic in the broker.

Pag 17

16/04/2025

User Manual – MQTT Device

2.2  MQTT Client in Easergy Builder

At the left side in the configuration view of Easergy Builder, there is a Devices tree for the
configuration.

Use the button

 or the right-button of the mouse (on the tree) for creating a new Device

Figure 7  – New Device.

Where:

•  Type: Type of the new Device. For MQTT Client select 'MQTT'.

•  Name: Name of the new Device (Only letter, numbers and ‘_’ character are allowed for the

name).

•  Description (optional): Description of the new Device.

Pag 18

User Manual – MQTT Device

16/04/2025

2.2.1

Device Configuration

For the MQTT Device it is not necessary to configure any channel, since the MQTT device in the
RTU created the channel automatically.

Figure 8  – MQTT Broker configuration.

In the Device configuration window, the following information is available:

•

ID: In the previous example, the device will connect to the broker with the name hu250val.

•  QoS: Determines the Quality of Service of the communication with the broker. It can be:

o  At most once

o  At least once

o  Exactly once

•  Version: The versions of MQTT supported to be configured are:

o  3.1.1

o  5

•  User: User to access the broker. As this parameter is not configurable through EB, it does not

appear.

•  Pass: Password to access the broker. As this parameter is not configurable through EB, it

does not appear.

•  URL: URL type (IPv4 or IPV6) and URL address of the broker.

•

Interval: Interval, in milliseconds, to publish and subscribe to topics. Minimum value is 50.

•  TLS: Enable or disable TLS encryption.

•  Port: Port to connect to the broker.

Pag 19

16/04/2025

User Manual – MQTT Device

•  Sparkplug: Enable or disable Sparkplug specification.

•  Group: Group for Sparkplug specification.

Once the broker connection is configured, clicking on the “Topics” button on the left panel of the
MQTT – Configuration window the topics can be configured.

Figure 11  – Topics configuration.

Topics are defined here, but the subscription and publication to any of them is configured later
in CoreDB.

NOTICE

Topics can be configured with three parameters:

•  Value: Value of the topic. For example “Abc/123”.

•

ID: Id used to identify the topic later in CoreDB. For example “t1”.

•  Format: Format for the messages of the topic. It can be XML or JSON.

Pag 20

User Manual – MQTT Device

16/04/2025

Index of Figures

Figure 1  – Baseline Software Platform ........................................................................................................................ 9

Figure 2  – Relation between coreDb and other applications. ...................................................................................... 9

Figure 3  – Startup window of Easergy Builder. ......................................................................................................... 11

Figure 4  – Easergy Builder on WorkSpace mode. .................................................................................................... 11

Figure 5  – Configuration mode. ................................................................................................................................. 12

Figure 6  – Device catalog. ......................................................................................................................................... 13

Figure 9  – New Device. ............................................................................................................................................. 18

Figure 10  – MQTT Broker configuration. ................................................................................................................... 19

Pag 21

16/04/2025

Index of Tables

User Manual – MQTT Device

Table 1 – Reference Documents .................................................................................................................................. 2

Table 2 – Software versions ......................................................................................................................................... 2

Table 3 – Hardware / Software compatibility ................................................................................................................ 2

Table 4 – Symbols ........................................................................................................................................................ 4

Pag 22

User Manual – MQTT Device

Glossary

16/04/2025

A

AC: Alternate Current.

B

Bps: Bits per second.

D

DC: Direct Current.

H

HU: Head Unit. Saitel DR CPU.

HU_A: Saitel DR Advanced Head Unit.

HU_AF: Saitel DR Advanced Head Unit with acquisition.

HU_B: Saitel DR Basic Head Unit.

HU_BI: Saitel DR Basic Head Unit with acquisition.

HU250: PowerLogic T300 CPU.

HUe: Saitel DR High-Performance Head Unit.

I

IED: Intelligent Electronic Device.

I/O: Input / Output.

ISO 9001: International standard for Quality Systems.

M

MQTT: Message Queuing Telemetry Transport

N

N/A: Non-Application.

P

PC: Personal Computer.

R

RoHS: Restriction of Hazardous Substances.

RTU: Remote Terminal Unit.

S

s: Second.

SCADA: Supervisory Control And Data Acquisition.

SM_CPU866: Saitel DP CPU.

Pag 23

16/04/2025

User Manual – MQTT Device

SM_CPU866e: Saitel DP high-performance CPU.

SSH: Secure SHell.

T

TCP/IP: Transmission Control Protocol/Internet Protocol.

W

WEEE: Waste Electrical and Electronic Equipment.

Pag 24

 Printed in:

Tuesday, March 17, 2026

Schneider Electric

C/ Charles Darwin s/n
Parque Científico y Tecnológico de la Cartuja
Seville, Spain

©2025 All rights reserved. The information contained in this document is
confidential and is owned by Schneider Electric. It cannot be copied or distributed
in any way, unless there is express written authorization by Schneider Electric.
Although this information was verified at the time of publication, may be subject to change without notice.

SE-MQTT-S854-1.0   04/2025

