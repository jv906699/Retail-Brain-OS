<p align="center">
&#x20; <img
&#x20;   src="https\://capsule-render.vercel.app/api?type=waving&color=0:0f172a,25:0ea5e9,50:06b6d4,75:8b5cf6,100\:ec4899&height=220&section=header&text=RETAIL%20BRAIN%20OS&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=34&desc=AI-POWERED%20RETAIL%20INTELLIGENCE%20PLATFORM&descSize=17&descAlignY=56&descColor=ffffff"
&#x20;   width="100%"
&#x20;   alt="Retail Brain OS"
&#x20; />
</p>
<p align="center">
&#x20; <img
&#x20;   src="https\://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=900&color=0EA5E9&center=true&vCenter=true&repeat=true&width=720&height=32&lines=Turning+CCTV+into+Retail+Intelligence;Real-Time+Computer+Vision;Person+Detection+%7C+Tracking+%7C+Zone+Intelligence;Dwell-Time+%7C+Customer+Sessions+%7C+Event+Processing;From+Visual+Data+to+Business+Insights"
&#x20;   alt="Retail Brain OS capabilities"
&#x20; />
</p>
<p align="center">
&#x20; <kbd>COMPUTER VISION</kbd>
&#x20; &nbsp;&nbsp;
&#x20; <kbd>REAL-TIME AI</kbd>
&#x20; &nbsp;&nbsp;
&#x20; <kbd>RETAIL INTELLIGENCE</kbd>
&#x20; &nbsp;&nbsp;
&#x20; <kbd>EDGE AI</kbd>
</p>
<br>

Retail Brain OS is an AI-powered retail intelligence platform designed to transform existing CCTV infrastructure into a real-time store intelligence system.

The platform combines computer vision, person detection, multi-object tracking, configurable store zones, customer movement analysis, dwell-time intelligence, event generation, and a live operational dashboard.
Instead of treating CCTV footage as passive video, Retail Brain OS converts live visual information into structured customer-activity data that can help retailers understand how customers move and interact within their stores.

🧭 Vision

The long-term vision of Retail Brain OS is to build a Retail Intelligence Operating System for Indian retailers.
The platform is designed to transform existing CCTV infrastructure into a business intelligence layer without requiring retailers to replace their existing camera infrastructure.

Retail Intelligence Capability Matrix

Capability

What the platform is designed to understand

👣 Customer Movement

Customer movement patterns

🔁 Visitor Behavior

Repeat visitor behavior and returning frequency

🏪 Store Occupancy

Occupancy and peak business hours

🎯 Product Interest

Activity within product-interest zones

🚶 Queue Behavior

Activity around waiting and checkout areas

🧠 Customer Intent

Customer intent trends derived from observed activity

📊 Store Analytics

Store performance analytics

Privacy-oriented design: The system is designed around anonymous customer activity rather than permanent personal identification or storage of sensitive biometric identities.

🎯 Product Positioning

AI-Powered Retail Growth Intelligence Platform

Retail Brain OS is being developed as a plug-and-play intelligence layer for retail environments.

Existing Infrastructure Compatibility

Existing Infrastructure

Role in the platform

📹 CCTV Cameras

Visual data source

🌐 IP Cameras

Network camera input

💾 DVR Systems

Existing video infrastructure

🗄️ NVR Systems

Network video recording infrastructure

🏬 Retail Infrastructure

Existing store environment

The goal is to make advanced computer-vision-based retail intelligence accessible without requiring expensive new surveillance hardware.

🧠 Current Implementation

The current implementation represents the computer-vision and edge-intelligence foundation of the larger Retail Brain OS platform.
It provides a working real-time pipeline that can process camera/video input, detect and track people, understand configurable store zones, calculate customer dwell time, generate customer activity events, and present the resulting intelligence through a live graphical interface.

Current Intelligence Stack

Layer

Current capability

Visual Input

Camera / video processing

Computer Vision

Person detection

Tracking

Anonymous multi-object tracking

Spatial Intelligence

Configurable store zones

Temporal Intelligence

Dwell-time analysis

Session Intelligence

Visitor session state

Event Processing

Customer and zone events

Presentation

Live Retail Brain OS GUI

The current system is therefore the foundational edge layer upon which the broader Retail Brain OS product vision can be built.

🏗️ System Overview

Current Retail Brain OS Pipeline

The current implementation follows a modular real-time computer-vision pipeline that transforms camera/video input into structured retail intelligence.

<p align="center">
&#x20; <img
&#x20;   src="https\://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=900&color=06B6D4&center=true&vCenter=true&repeat=true&width=760&height=36&lines=CAMERA+%E2%86%92+FRAME+CAPTURE+%E2%86%92+PERSON+DETECTION;PERSON+DETECTION+%E2%86%92+MULTI-OBJECT+TRACKING;TRACKING+%E2%86%92+ANONYMOUS+TRACK+IDs+%E2%86%92+ZONE+INTELLIGENCE;ZONE+INTELLIGENCE+%E2%86%92+DWELL-TIME+ANALYSIS;CUSTOMER+SESSIONS+%E2%86%92+STRUCTURED+EVENTS+%E2%86%92+LIVE+RETAIL+OS"
&#x20;   alt="Retail Brain OS animated pipeline"
&#x20; />
</p>
<p align="center">
&#x20; <kbd>CAMERA</kbd> → <kbd>DETECTION</kbd> → <kbd>TRACKING</kbd> → <kbd>ZONES</kbd> → <kbd>DWELL</kbd> → <kbd>EVENTS</kbd> → <kbd>LIVE GUI</kbd>
</p>
<p align="center">
&#x20; <sub>From live CCTV input to structured retail intelligence in real time.</sub>
</p>

Core Processing Flow

Stage

Input

Processing

Result

1. Camera / Video Input

Live camera or video

Continuous frame capture

Incoming frames

2. Person Detection

Video frames

Object-detection pipeline

Person locations

3. Multi-Object Tracking

Detections

Tracking across frames

Anonymous track IDs

4. Zone Intelligence

Tracks + polygons

Zone state analysis

Zone entry / presence / exit

5. Dwell-Time Intelligence

Zone state

Duration measurement

Dwell metrics

6. Customer Session

Visitor state

Session aggregation

Visitor session state

7. Event Generation

State changes

Structured event processing

Customer / zone events

8. Live Interface

Intelligence data

Visualization

Operational dashboard

Tracking State

Detected people receive temporary tracking IDs so continuity can be maintained across consecutive frames.

Example entity

Anonymous reference

Person

Track ID 1

Person

Track ID 2

Person

Track ID 3

These IDs allow Retail Brain OS to reason about movement during a store session without requiring a permanent personal identity.

Zone Intelligence

The system supports configurable polygon-based store zones.

Example zone

Possible retail meaning

Entrance

Store entry area

Product

Product/display area

Billing

Checkout area

Waiting

Waiting / queue area

Custom

Any retailer-defined region

The intelligence layer determines when a tracked person enters, remains inside, or leaves a configured zone.

Dwell-Time Intelligence

Dwell attribute

Meaning

Current zone dwell

Time currently spent in a zone

Total dwell

Accumulated observed dwell

Zone-wise dwell

Dwell broken down by zone

Zone visit history

Previously visited zones

This allows the system to understand not only where a customer moved, but also how long they spent in each area.

Customer Session Intelligence

A session-level representation can contain:

Session attribute

Purpose

Track ID

Anonymous visitor reference

First seen time

First observed timestamp

Store entry time

Entry timestamp

Store exit time

Exit timestamp

Current status

Current visitor state

Current zone

Current location

Total dwell time

Total observed dwell

Zone-wise dwell time

Time spent by zone

Zone visit history

Sequence of visited zones

Event Generation

Event

Meaning

Customer entry

Visitor enters the monitored environment

Zone entry

Visitor enters a configured zone

Zone exit

Visitor leaves a configured zone

Customer exit

Visitor leaves the monitored environment

These events form the bridge between raw computer-vision output and higher-level retail intelligence.

🧩 Modular Architecture

The current implementation separates the major responsibilities into independent components.

Layer

Responsibilities

Vision Layer

Detection · Tracking · Frame Processing

Intelligence Layer

Zones · Entry / Exit · Dwell · Customer Sessions

Presentation Layer

Retail Brain OS GUI

This separation allows the vision pipeline and intelligence logic to operate independently from the presentation layer.

🚀 Core Features

1. Live Camera & Real-Time AI Detection

Retail Brain OS provides a live visual interface for monitoring a camera or video source while simultaneously processing incoming frames through the computer-vision pipeline.

Live Camera Capability Matrix

Capability

Purpose

Camera / video visualization

Display the live visual source

Person detection

Identify people in incoming frames

Bounding boxes

Visualize detections

Anonymous tracking IDs

Maintain visitor continuity

Confidence information

Expose detection confidence

Zone visualization

Display configured analytical regions

Continuous processing

Process incoming frames

Live FPS

Runtime performance visibility

Camera resolution

Input visibility

Runtime status

Operational state visibility

Real-Time Processing Flow

Step

Processing

01

Camera / Video Frame

02

Frame Processing

03

Person Detection

04

Tracking

05

Track ID Assignment

06

Zone Analysis

07

Retail Intelligence

08

Live GUI

📸 Live Camera & AI Detection

<img width="1919" height="1079" alt="image" src="https\://github.com/user-attachments/assets/9e541726-c095-4b0f-9cec-c64e6cb0ec0a" />
The live interface provides simultaneous visibility into the camera feed, detected people, tracking IDs, configured zones, runtime performance, and generated retail intelligence.

📊 Retail Intelligence Dashboard

Retail Brain OS transforms the live camera stream into an operational retail intelligence interface.
Instead of displaying only raw detections, the system derives information about people, zones, movement, dwell time, entry/exit activity, and the current state of the store.

Live Intelligence Overview

Dashboard Metric

Meaning

People currently inside

Current tracked visitors

Total entries

Cumulative store entries

Total exits

Cumulative store exits

Active zones

Zones with current tracked activity

Zone-wise dwell

Visitor time spent within zones

Active tracked people

Currently active visitors

Recent events

Latest customer movement events

Selected person

Detailed state of a selected visitor

📸 Live Intelligence Dashboard

<p align="center">
&#x20; <img width="275" height="506" alt="image" src="https\://github.com/user-attachments/assets/c6b6b850-f004-44d2-ab3f-435694e43be2" />
</p>
<p align="center">
&#x20; <img width="290" height="574" alt="image" src="https\://github.com/user-attachments/assets/0d02b3ca-415d-45e2-9f3b-643501e48a53" />
</p>
The dashboard updates these values while the vision pipeline is running, allowing the operator to observe customer activity without manually reviewing the camera feed frame-by-frame.

🏪 Store Occupancy Intelligence

Retail Brain OS maintains an understanding of the people currently present within the monitored store environment.
The People in Store metric represents the current number of tracked visitors considered to be inside the monitored environment. This differs from simply counting detections in an individual frame.

Occupancy Metrics

Metric

Represents

People in Store

Current occupancy

Total Entered

Cumulative store entries

Total Exited

Cumulative store exits

These metrics provide an immediate operational view of customer traffic.

📸 Occupancy Metrics

<img width="294" height="450" alt="image" src="https\://github.com/user-attachments/assets/f0472f2b-7bd6-4426-9ebd-af84ead4d69e" />

🎯 Zone Intelligence

Zone-Based Retail Intelligence

Zone Intelligence is a core component of Retail Brain OS. Operators can define custom areas within the camera view and analyze customer activity inside those regions.

Supported Zone Types

Zone

Example use

Product section

Product-area activity

Display area

Display engagement

Checkout area

Billing / checkout activity

Promotional section

Promotion-area activity

Waiting area

Queue / waiting activity

High-value product zone

High-value product activity

Custom zone

Retailer-defined analytical region

Each configured zone becomes an independent region for activity analysis.

Zone Processing

Capability

Description

Polygon configuration

Define custom analytical boundaries

Zone identity

Give each zone a distinct name

Zone entry

Detect tracked visitors entering

Zone presence

Maintain current zone state

Zone exit

Detect tracked visitors leaving

Zone history

Preserve visited-zone information

📸 Configured Zones

<img width="1336" height="793" alt="Screenshot 2026-08-17 213005" src="https\://github.com/user-attachments/assets/4aa55273-dd73-4ea0-83b0-adf1aadd8767" />
Configured zones are displayed directly over the live camera feed using colored polygon boundaries, making the relationship between the physical camera environment and analytical regions immediately visible.

⏱️ Zone-Wise Dwell Time

Retail Brain OS measures how long tracked visitors remain within configured zones.
Dwell time adds behavioral context beyond simple visitor counting.

Dwell Intelligence Model

Attribute

Description

Current dwell

Time currently spent in the active zone

Total dwell

Accumulated visitor dwell

Zone-wise dwell

Dwell separated by zone

Visitor history

Dwell accumulated across the session

Example Session

Visitor

Zone

Current Dwell

State

Track ID 1

Zone B

02:15

Active

The example above illustrates the structure documented by the project; it is not presented as a live system measurement.

📸 Zone-Wise Dwell

<img width="272" height="122" alt="image" src="https\://github.com/user-attachments/assets/4386196e-1959-4293-b3f4-57d8f024f0f9" />

👥 Active People Intelligence

The dashboard maintains a live list of currently active tracked people.

Active-person field

Information

Anonymous Track ID

Temporary visitor reference

Current zone

Current analytical region

Current dwell time

Time spent in the current zone

📸 Active People

<img width="277" height="149" alt="image" src="https\://github.com/user-attachments/assets/33d6afe3-1185-455d-9c4d-5a5ad0ac6aa2" />
Selecting an active person provides access to more detailed information about that tracked session.

🧾 Individual Customer Session Intelligence

Retail Brain OS maintains a session-level intelligence record for each tracked visitor.
When an active person is selected, the PERSON DETAILS (SELECTED) panel provides information about that individual's activity during the current session.

Session Detail Model

Attribute

Description

Anonymous Track ID

Temporary visitor reference

First-seen time

First observation

Current zone

Current location

Current dwell time

Current zone duration

Total dwell time

Accumulated dwell

Store presence state

Current store state

This allows the operator to inspect an individual visitor without exposing a permanent personal identity.

📸 Selected Person Details

<img width="261" height="201" alt="image" src="https\://github.com/user-attachments/assets/352db391-69fe-42e7-8591-d812bc512b3f" />
The selected-person view connects the visitor's tracking state with the higher-level retail intelligence generated by the system.

🗺️ Multi-Zone Customer Journey

Retail Brain OS does not treat a visitor's activity as a single-zone event.
A tracked visitor can move between multiple configured zones during the same session, while the intelligence layer maintains zone visit information and accumulates dwell time across visited zones.

Example Journey

Visitor ID 1
     │
     ▼
   Zone B
     │
     ▼
   Zone A
     │
     ▼
   Zone B
     │
     ▼
 Store Exit

Journey Intelligence

Journey information

Purpose

Zone sequence

Understand movement between areas

Zone visits

Record visited regions

Zone-wise dwell

Measure time by region

Store exit

Close the observed session

This provides a foundation for understanding how visitors move through different areas rather than only measuring total store occupancy.

🚪 Customer Entry & Exit Intelligence

Retail Brain OS tracks customer movement into and out of the monitored environment.
The intelligence layer generates entry and exit events and maintains cumulative counts for the current operational session.

Entry / Exit Metrics

MetricMeaning



Total Entered

Total visitors who entered

Total Exited

Total visitors who exited

People in Store

Visitors currently inside

📸 Entry & Exit Metrics

<img width="269" height="172" alt="image" src="https\://github.com/user-attachments/assets/04e81ace-f342-4fe6-9ade-91a179dccc59" />
This allows the operator to distinguish between total visitors who entered, visitors who have exited, and visitors currently inside.

⚡ Real-Time Event Stream

Retail Brain OS maintains a recent event stream so important customer movement events can be observed without manually inspecting the video.

Event Types

Event

Description

🟢 Customer entered

Visitor entered the store

🔴 Customer exited

Visitor exited the store

🔵 Zone entered

Visitor entered a configured zone

🟠 Zone exited

Visitor exited a configured zone

Each event is associated with the relevant anonymous tracking ID and timestamp.

📸 Recent Events

<img width="280" height="98" alt="image" src="https\://github.com/user-attachments/assets/d476d544-c89e-4610-8828-e78ca075f987" />
The event stream provides a chronological operational view of recent customer activity.

🖥️ Live Vision Runtime Monitoring

Retail Brain OS exposes runtime information alongside the retail intelligence layer.

Runtime Telemetry

Runtime signal

Purpose

Runtime status

Current processing state

FPS

Frame-processing performance

Processing time

Processing latency visibility

Frame number

Current frame state

Configured zones

Number of active zones

Runtime errors

Operational error visibility

Camera connection

Input connection state

Tracker state

Tracking state

Loaded zones

Currently loaded analytical regions

📸 Runtime Monitoring

<p align="center">
&#x20; <img width="277" height="202" alt="Screenshot 2026-08-17 215714" src="https\://github.com/user-attachments/assets/e99e48be-228c-4059-84c3-0f5702d461a3" />
</p>
<p align="center">
&#x20; <img width="1901" height="39" alt="Screenshot 2026-08-17 215727" src="https\://github.com/user-attachments/assets/14a99314-f1df-420c-974c-2b5b3557b9f2" />
</p>

🎛️ Retail Operations & Control Interface

Retail Brain OS is designed as an operational interface rather than a passive monitoring screen.
The GUI provides dedicated controls for configuring the retail environment, controlling the live vision runtime, managing surveillance recordings, capturing data, and accessing previously saved information.

Operational Areas

Area

Responsibility

Zone Setup & Configuration

Configure analytical regions

Live Intelligence & Monitoring

Observe current retail activity

Runtime Control Panel

Control the active system

Zone Setup & Configuration

The left-side dashboard provides the controls required to configure the analytical environment before running the Retail Brain OS vision pipeline.

Zone Configuration Data

Field

Purpose

Selected zone

Currently selected analytical region

Polygon points

Geometry of the configured zone

Zone area

Area represented by the polygon

Last updated

Latest zone configuration information

📸 Zone Configuration

<img width="263" height="785" alt="image" src="https\://github.com/user-attachments/assets/7d6b702a-a86a-4479-bfe1-f59179409379" />

🎛️ Runtime Control Panel

The bottom control panel provides direct operational controls for Retail Brain OS.

Control

Purpose

Setup Zones

Opens the zone configuration workflow

Start Retail OS

Starts the live Retail Brain OS runtime

Stop Retail OS

Stops the active runtime

Record Surveillance

Starts surveillance recording

Stop Recording

Stops the active recording

Capture Face

Captures and saves a visitor image when required

Save Data

Saves current operational intelligence data

Open Saved Files

Opens previously saved operational data

Close

Closes the current Retail Brain OS interface

📸 Control Panel

<img width="1915" height="460" alt="image" src="https\://github.com/user-attachments/assets/3d647453-45b0-420a-ba96-dbecbc5804d8" />
The control panel provides a single operational area from which the operator can control the major runtime and data-management functions of the system.

💾 Saved Data & Recorded Sessions

Retail Brain OS provides mechanisms for preserving information generated during operation.

Capability

Purpose

Save Data

Preserve current operational intelligence

Open Saved Files

Access previously saved information

Session information

Preserve tracked visitor movement and dwell information

Surveillance recording

Preserve the camera stream when required

📸 Data & Recording Controls

<img width="1068" height="43" alt="image" src="https\://github.com/user-attachments/assets/418fd3f1-e136-4ceb-83d3-f68d88500ac5" />

📡 System Status Monitoring

A persistent status bar at the bottom of the interface provides a high-level overview of the current system state.

Status Indicators

Indicator

Represents

Overall system status

Current application state

Camera connection

Camera/input connectivity

Tracker state

Tracking subsystem state

Loaded zones

Currently loaded analytical regions

Retail Brain OS version

Current application version

📸 System Status

<img width="1913" height="38" alt="image" src="https\://github.com/user-attachments/assets/714cc6b4-234b-4617-b47c-6c728de35cf1" />
This provides immediate operational feedback without requiring the operator to inspect individual dashboard panels.

🔍 System Capability Summary

Area                   Capabilities

Computer Vision        Person detection · frame processing

Tracking               Anonymous multi-object tracking

Spatial Intelligence   Polygon zones · zone entry · zone exit

Temporal Intelligence  Current dwell · total dwell · zone-wise dwell

Customer Intelligence  Sessions · active people · multi-zone journeys

Event Processing       Customer entry · customer exit · zone events

Dashboard              Occupancy · active zones · dwell · recent events

Runtime Monitoring     FPS · processing time · camera state · tracker state

Operations             Zone setup · runtime control · recording · data management

<p align="center">
&#x20; <sub>Retail Brain OS — transforming existing CCTV infrastructure into structured retail intelligence.</sub>
</p>
