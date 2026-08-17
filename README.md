# Retail Brain OS

### AI-Powered Retail Intelligence & Surveillance System

Retail Brain OS is an AI-powered retail intelligence platform designed to transform existing CCTV infrastructure into a real-time store intelligence system.

The platform combines computer vision, person detection, multi-object tracking, configurable store zones, customer movement analysis, dwell-time intelligence, event generation, and a live operational dashboard.

Instead of treating CCTV footage as passive video, Retail Brain OS converts live visual information into structured customer-activity data that can help retailers understand how customers move and interact within their stores.

---

## Vision

The long-term vision of Retail Brain OS is to build a **Retail Intelligence Operating System** for Indian retailers.

The platform is designed to transform existing CCTV infrastructure into a business intelligence layer without requiring retailers to replace their existing camera infrastructure.

The broader product vision is to help retailers understand:

- Customer movement patterns
- Repeat visitor behavior
- Store occupancy and peak business hours
- Product interest zones
- Queue behavior
- Customer intent trends
- Returning customer frequency
- Store performance analytics

The system is designed around anonymous customer activity rather than permanent personal identification or the storage of sensitive biometric identities.

---

## Product Positioning

### AI-Powered Retail Growth Intelligence Platform

Retail Brain OS is being developed as a plug-and-play intelligence layer for retail environments.

The intended platform is designed to work with existing:

- CCTV cameras
- IP cameras
- DVR systems
- NVR systems
- Retail infrastructure

The goal is to make advanced computer-vision-based retail intelligence accessible without requiring expensive new surveillance hardware.

---

## Current Implementation

The current implementation represents the **computer-vision and edge-intelligence foundation** of the larger Retail Brain OS platform.

It provides a working real-time pipeline that can process camera/video input, detect and track people, understand configurable store zones, calculate customer dwell time, generate customer activity events, and present the resulting intelligence through a live graphical interface.

The current system is therefore the foundational edge layer upon which the broader Retail Brain OS product vision can be built.

---

# System Overview

## Current Retail Brain OS Pipeline

The current implementation follows a modular real-time computer vision pipeline that transforms camera/video input into structured retail intelligence.

Camera / Video Source
        │
        ▼
   Frame Capture
        │
        ▼
 Person Detection
        │
        ▼
 Multi-Object Tracking
        │
        ▼
 Anonymous Track IDs
        │
        ▼
   Zone Intelligence
        │
        ├───────────────┐
        ▼               ▼
 Zone Entry        Zone Exit
 Detection         Detection
        │               │
        └───────┬───────┘
                ▼
        Dwell-Time Analysis
                │
                ▼
       Customer Session
          Intelligence
                │
                ▼
        Structured Events
                │
                ▼
       Live Retail OS GUI

Core Processing Flow
1. Camera / Video Input

Retail Brain OS accepts a live visual stream as the input to the vision pipeline.

The current implementation can operate with camera/video input and continuously process incoming frames.

2. Person Detection

Each processed frame is passed through the object-detection pipeline to identify people.

The detection stage provides the information required by the tracking and intelligence layers, including the detected person's location within the frame.

3. Multi-Object Tracking

Detected people are assigned temporary tracking IDs so that the system can maintain continuity across consecutive frames.

For example:
Person → Track ID 1
Person → Track ID 2
Person → Track ID 3

These IDs allow Retail Brain OS to reason about the movement of individual anonymous visitors during a store session.

4. Zone Intelligence

The system supports configurable polygon-based store zones.

A retailer can define areas such as:

Entrance areas
Product areas
Billing areas
Waiting areas
Other custom store regions

The intelligence layer determines when a tracked person enters, remains inside, or leaves a configured zone.

5. Dwell-Time Intelligence

When a tracked person spends time inside a zone, Retail Brain OS measures the duration of that visit.

The system maintains:

Current zone dwell time
Total dwell time
Zone-wise dwell time
Zone visit history

This allows the system to understand not only where a customer moved, but also how long they spent in each area.

6. Customer Session Intelligence

The system maintains a session-level representation of tracked visitors.

A session can contain information such as:

Track ID
First seen time
Store entry time
Store exit time
Current status
Current zone
Total dwell time
Zone-wise dwell time
Zone visit history

This information can then be presented through the Retail Brain OS interface.

7. Event Generation

The intelligence layer generates structured events from the customer's movement through the store.

Examples include:

Customer entry
Zone entry
Zone exit
Customer exit

These events form the bridge between raw computer-vision output and higher-level retail intelligence.

8. Live Retail Brain OS Interface

The processed intelligence is presented through the live GUI.

The interface provides the operator with real-time visibility into:

Active people
Tracking IDs
Current zones
Dwell information
Store activity
Camera status
System status
Customer session information

The GUI also provides tools for recording, face capture, saving session data, and reviewing previously captured information.

Modular Architecture

The current implementation separates the major responsibilities of the system into independent components.

Vision Layer
    │
    ├── Detection
    ├── Tracking
    └── Frame Processing
            │
            ▼
Intelligence Layer
    │
    ├── Zones
    ├── Entry / Exit
    ├── Dwell
    └── Customer Sessions
            │
            ▼
Presentation Layer
    │
    └── Retail Brain OS GUI

    This separation allows the vision pipeline and intelligence logic to operate independently from the presentation layer.

It also provides a foundation for the larger Retail Brain OS architecture described in the project's long-term product vision.

---

# Core Features

## 1. Live Camera & Real-Time AI Detection

Retail Brain OS provides a live visual interface for monitoring a camera or video source while simultaneously processing the incoming frames through the computer-vision pipeline.

As frames are received, the system performs real-time person detection and tracking. Detected people are represented directly on the camera view, allowing the operator to observe the AI system's interpretation of the scene.

The live camera interface provides immediate visual feedback while the intelligence pipeline processes customer movement in the background.

### What the Live Camera View Provides

- Real-time camera/video visualization
- Person detection
- Bounding-box visualization
- Anonymous tracking IDs
- Confidence information
- Configured zone visualization
- Continuous frame processing
- Live FPS information
- Camera resolution information
- Runtime status information

### Real-Time Processing Flow

Camera / Video Frame
        ↓
Frame Processing
        ↓
Person Detection
        ↓
Tracking
        ↓
Track ID Assignment
        ↓
Zone Analysis
        ↓
Retail Intelligence
        ↓
Live GUI

The live camera view therefore acts as the primary visual interface between the physical retail environment and the Retail Brain OS intelligence pipeline.

It allows an operator to see the detected customers, their tracking IDs, their position within the store, and the configured intelligence zones while the system is running.

Operational Visibility

The interface also exposes live system information so that the operator can understand the current state of the runtime while the vision pipeline is active.

This includes camera-related information such as frame processing, resolution, and runtime status.

Live Camera & AI Detection

Screenshot: The image below shows Retail Brain OS processing a live camera/video stream with detected and tracked people, configured zones, and the live operational interface.

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/9e541726-c095-4b0f-9cec-c64e6cb0ec0a" />
The live interface provides simultaneous visibility into the camera feed, detected people, tracking IDs, configured zones, runtime performance, and generated retail intelligence.

---

# Retail Intelligence Dashboard

Retail Brain OS transforms the live camera stream into an operational retail intelligence interface.

Instead of displaying only raw detections, the system continuously derives information about people, zones, movement, dwell time, entry/exit activity, and the current state of the store.

The dashboard is designed to give an operator a real-time view of what is happening inside the monitored environment.

## Live Intelligence Overview

The right-side intelligence panel provides a continuously updated summary of the current retail environment.

It exposes key operational metrics including:

- People currently inside
- Total entries
- Total exits
- Active zones
- Zone-wise dwell activity
- Active tracked people
- Recent events
- Selected-person information

### 📸 Screenshot — Live Intelligence Dashboard

<img width="275" height="506" alt="image" src="https://github.com/user-attachments/assets/c6b6b850-f004-44d2-ab3f-435694e43be2" />

<img width="290" height="574" alt="image" src="https://github.com/user-attachments/assets/0d02b3ca-415d-45e2-9f3b-643501e48a53" />

The dashboard updates these values while the vision pipeline is running, allowing the operator to observe customer activity without manually reviewing the camera feed frame-by-frame

---

## Store Occupancy Intelligence

Retail Brain OS maintains an understanding of the people currently present within the monitored store environment.

The **People in Store** metric represents the current number of tracked visitors considered to be inside the monitored environment.

This is different from simply counting detections in a frame.

The intelligence layer maintains the state of tracked people and uses their movement and store entry/exit state to determine whether they are currently inside.

### Key Metrics

People in Store
      ↓
Current occupancy

Total Entered
      ↓
Cumulative store entries

Total Exited
      ↓
Cumulative store exits

These metrics provide an immediate operational view of customer traffic.

📸 Screenshot — Occupancy Metrics

<img width="294" height="450" alt="image" src="https://github.com/user-attachments/assets/f0472f2b-7bd6-4426-9ebd-af84ead4d69e" />


---

# Phase 5 — Zone Intelligence

This is one of the **most important features of our project**, so give it more space.

## Zone-Based Retail Intelligence

Retail Brain OS allows operators to define custom areas within the camera view and analyze customer activity inside those areas.

Zones can represent meaningful retail locations such as:

- Product sections
- Display areas
- Checkout areas
- Promotional sections
- Waiting areas
- High-value product zones

Each configured zone becomes an independent region for activity analysis.

The system continuously determines which tracked people are interacting with each configured zone.

### Zone Visualization

Configured zones are displayed directly over the live camera feed using colored polygon boundaries.

Each zone has its own name and visual identity, allowing the operator to distinguish multiple areas simultaneously.

### 📸 Screenshot — Configured Zones

<img width="1336" height="793" alt="Screenshot 2026-08-17 213005" src="https://github.com/user-attachments/assets/4aa55273-dd73-4ea0-83b0-adf1aadd8767" />

The visualization makes the relationship between the physical camera environment and the configured analytical zones immediately visible.


---

# Phase 6 — Zone-Wise Dwell Time

This is another **core intelligence feature**.

## Zone-Wise Dwell Time

Retail Brain OS measures how long tracked visitors remain within configured zones.

Dwell time provides an additional layer of behavioral intelligence beyond simple visitor counting.

For each active zone, the dashboard can display the tracked person associated with that zone together with their current dwell duration.

### Example
Zone B
ID: 1
Dwell: 02:15
This allows the operator to identify areas where visitors are spending more time.

The system also maintains dwell information at the individual visitor level, allowing activity to be analyzed across multiple zones during a session.

📸 Screenshot — Zone-Wise Dwell

<img width="272" height="122" alt="image" src="https://github.com/user-attachments/assets/4386196e-1959-4293-b3f4-57d8f024f0f9" />


---

# Phase 7 — Active People Intelligence

## Active People

The dashboard maintains a live list of currently active tracked people.

For each active person, the interface can display:

- Anonymous tracking ID
- Current zone
- Current dwell time

This allows the operator to quickly understand who is currently active and where they are located within the monitored environment.

### 📸 Screenshot — Active People

<img width="277" height="149" alt="image" src="https://github.com/user-attachments/assets/33d6afe3-1185-455d-9c4d-5a5ad0ac6aa2" />
Selecting an active person provides access to more detailed information about that tracked session.

Phase 8 — Individual Customer Session Intelligence

This is where our implementation becomes much more interesting than a normal detection dashboard.

---


## Individual Customer Session Intelligence


Retail Brain OS maintains a session-level intelligence record for each tracked visitor.


When an active person is selected, the **PERSON DETAILS (SELECTED)** panel provides information about that individual's activity during the current session.


Depending on the visitor's current state, the interface can expose information such as:


- Anonymous Track ID
- First-seen time
- Current zone
- Current dwell time
- Total dwell time
- Store presence state


This allows the operator to inspect an individual visitor without exposing a permanent personal identity.


### 📸 Screenshot — Selected Person Details

<img width="261" height="201" alt="image" src="https://github.com/user-attachments/assets/352db391-69fe-42e7-8591-d812bc512b3f" />
The selected-person view connects the visitor's tracking state with the higher-level retail intelligence generated by the system.

---

## Multi-Zone Customer Journey

Retail Brain OS does not treat a visitor's activity as a single-zone event.

A tracked visitor can move between multiple configured zones during the same session.

The intelligence layer maintains zone visit information and accumulates dwell time across the zones visited by that person.

For example:
Visitor ID 1

Zone B
   ↓
Zone A
   ↓
Zone B
   ↓
Store Exit

The system can maintain the corresponding zone-wise dwell information for that visitor.
This provides a foundation for understanding how visitors move through different areas of a retail environment rather than only measuring total store occupancy.


# Phase 10 — Entry & Exit Intelligence

## Customer Entry & Exit Intelligence

Retail Brain OS tracks customer movement into and out of the monitored environment.

The intelligence layer generates entry and exit events and maintains cumulative counts for the current operational session.

The dashboard exposes:

Total Entered
Total Exited
People in Store

<img width="269" height="172" alt="image" src="https://github.com/user-attachments/assets/04e81ace-f342-4fe6-9ade-91a179dccc59" />

This allows the operator to distinguish between:
Total visitors who entered
Visitors who have exited
Visitors currently inside

---

## Real-Time Event Stream

Retail Brain OS maintains a recent event stream so that important customer movement events can be observed without manually inspecting the video.

Events can include activities such as:

- Customer entered the store
- Customer exited the store
- Customer entered a zone
- Customer exited a zone

Each event is associated with the relevant anonymous tracking ID and timestamp.

### 📸 Screenshot — Recent Events

<img width="280" height="98" alt="image" src="https://github.com/user-attachments/assets/d476d544-c89e-4610-8828-e78ca075f987" />
The event stream provides a chronological operational view of recent customer activity.

---

## Live Vision Runtime Monitoring

Retail Brain OS exposes runtime information alongside the retail intelligence layer.

This allows the operator to understand whether the vision pipeline is actively processing the camera stream and how the runtime is performing.

The interface provides information such as:

- Runtime status
- FPS
- Processing time
- Frame number
- Number of configured zones
- Runtime errors
- Camera connection state
- Tracker state
- Loaded zones

### 📸 Screenshot — Runtime Monitoring

<img width="277" height="202" alt="Screenshot 2026-08-17 215714" src="https://github.com/user-attachments/assets/e99e48be-228c-4059-84c3-0f5702d461a3" />

<img width="1901" height="39" alt="Screenshot 2026-08-17 215727" src="https://github.com/user-attachments/assets/14a99314-f1df-420c-974c-2b5b3557b9f2" />

---

# Retail Operations & Control Interface

Retail Brain OS is designed as an operational interface rather than a passive monitoring screen.

The GUI provides dedicated controls for configuring the retail environment, controlling the live vision runtime, managing surveillance recordings, capturing data, and accessing previously saved information.

The interface is divided into three major operational areas:

- Zone Setup & Configuration
- Live Intelligence & Monitoring
- Runtime Control Panel
## Zone Setup & Configuration

The left-side dashboard provides the controls required to configure the analytical environment before running the Retail Brain OS vision pipeline.

### Zone Setup

The operator can create and configure custom zones directly for the current camera environment.

Configured zones are displayed in the **CONFIGURED ZONES** section, where the operator can manage the available zones.

The interface also provides **ZONE INFO**, which displays information about the currently selected zone.

This includes information such as:

- Selected zone
- Number of polygon points
- Zone area
- Last updated information

### 📸 Screenshot — Zone Configuration

<img width="263" height="785" alt="image" src="https://github.com/user-attachments/assets/7d6b702a-a86a-4479-bfe1-f59179409379" />

---

## Runtime Control Panel

The bottom control panel provides direct operational controls for Retail Brain OS.

It allows the operator to start and stop the retail intelligence runtime, control surveillance recording, capture visitor information, save operational data, access previously saved information, and exit the application.

### Available Controls

| Control | Purpose |
|---|---|
| Setup Zones | Opens the zone configuration workflow |
| Start Retail OS | Starts the live Retail Brain OS runtime |
| Stop Retail OS | Stops the active runtime |
| Record Surveillance | Starts surveillance recording |
| Stop Recording | Stops the active recording |
| Capture Face | Captures and saves a visitor image when required |
| Save Data | Saves the current operational intelligence data |
| Open Saved Files | Opens previously saved operational data |
| Close | Closes the current Retail Brain OS interface |

### 📸 Screenshot — Control Panel

<img width="1915" height="460" alt="image" src="https://github.com/user-attachments/assets/3d647453-45b0-420a-ba96-dbecbc5804d8" />
The control panel provides a single operational area from which the operator can control the major runtime and data-management functions of the system.

---

## Saved Data & Recorded Sessions

Retail Brain OS provides mechanisms for preserving information generated during operation.

The operator can save the current intelligence data and subsequently access previously saved information through the **OPEN SAVED FILES** control.

Saved visitor/session information can contain intelligence associated with tracked visitors, including their movement and dwell information.

The system also provides surveillance recording controls for preserving the camera stream when required.

### 📸 Screenshot — Data & Recording Controls

<img width="1068" height="43" alt="image" src="https://github.com/user-attachments/assets/418fd3f1-e136-4ceb-83d3-f68d88500ac5" />


---

# 5. System Status Bar

And this small thing at the very bottom should definitely be documented.

## System Status Monitoring

A persistent status bar at the bottom of the interface provides a high-level overview of the current system state.

It exposes information such as:

- Overall system status
- Camera connection
- Tracker state
- Loaded zones
- Retail Brain OS version

### 📸 Screenshot — System Status

<img width="1913" height="38" alt="image" src="https://github.com/user-attachments/assets/714cc6b4-234b-4617-b47c-6c728de35cf1" />
This provides immediate operational feedback without requiring the operator to inspect the individual dashboard panels






