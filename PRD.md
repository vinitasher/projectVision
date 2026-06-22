# Project Sentinel — Privacy-Preserving Semantic AR Glasses

**Version:** 0.1 | **Status:** Founder Concept / Pre-Seed Exploration | **Date:** June 2026

---

## Executive Summary

Project Sentinel is a privacy-first augmented reality platform built around a radical premise:

**AR glasses should understand the world without recording it.**

Current smart glasses largely depend on camera-first architectures that continuously capture visual information. While effective, these approaches introduce significant privacy concerns for both wearers and bystanders.

Sentinel uses a **Color LiDAR-first sensing architecture** combined with local AI to create a semantic understanding of the environment while minimizing collection and retention of personally identifiable information.

The system converts raw sensor inputs into a temporary semantic world model and discards underlying sensor data as quickly as possible.

---

## Core Thesis

Every major AR company is building products that place cameras on people's faces.

We believe society will increasingly push back against continuous visual surveillance.

The winning AR platform may be one that:

- Understands the world
- Assists the user
- Preserves privacy
- Maintains social acceptability

**Rather than storing photos and videos, Sentinel stores meaning.**

---

## Why LiDAR?

**Traditional Cameras Capture:**
- Faces
- Text
- Screens
- Documents
- License plates
- Clothing
- Personal appearance

**LiDAR Captures:**
- Geometry
- Distance
- Shape
- Motion
- Spatial relationships

**Example:**

Instead of storing:
```
John standing next to a red couch.
```

Store:
```
Human       → Distance: 2.3m
Sofa        → Distance: 1.8m
```

This dramatically reduces privacy exposure.

---

## Product Vision

Create lightweight AR glasses that provide:

- Navigation
- Accessibility assistance
- Spatial memory
- Object awareness
- Contextual computing
- Ambient AI assistance

...while remaining **privacy-preserving by design.**

---

## Design Principles

| Principle | Description |
|-----------|-------------|
| **Geometry First** | Use depth and spatial understanding before imagery |
| **Privacy First** | Collect the minimum information necessary |
| **Local First** | Perform processing locally whenever possible |
| **Ephemeral First** | Discard raw sensor information immediately |
| **Explainability** | Users should understand what the system knows |
| **Human Dignity** | Never identify people by default |

---

## Product Goals

1. Deliver useful environmental intelligence without continuous video recording
2. Provide all-day wearable form factor
3. Achieve social acceptability
4. Create a new privacy-preserving AR platform
5. Enable future AI agents to interact with the physical world safely

## Non-Goals

Sentinel will **not** initially support:

- Social media streaming
- Continuous video recording
- Facial recognition
- Emotion detection
- Advertising analytics
- Surveillance use cases

---

## User Personas

### Accessibility Users
- **Needs:** Obstacle detection, navigation, environmental awareness
- **Example:** *"Guide me to Gate B12."*

### Travelers
- **Needs:** Navigation, airport assistance, spatial awareness

### Professionals
- **Needs:** Contextual reminders, meeting awareness, spatial productivity

### Parents
- **Needs:** Home awareness, safety monitoring, child location reminders

---

## Technical Architecture

### Gen 1 — Smartphone-Tethered

**Philosophy:** Leverage the smartphone as the primary compute device.

**Glasses handle:**
- Color LiDAR sensing
- IMU
- Eye tracking
- Display rendering
- Privacy enforcement
- Sensor preprocessing
- Hazard detection

**Smartphone handles:**
- SLAM
- Semantic scene understanding
- World model generation
- LLM inference
- Application runtime
- Storage & networking

**Advantages:** Faster time to market, lower BOM, better battery life, lower thermal risk
**Disadvantages:** Requires smartphone, limited standalone operation

### Gen 2 — Hybrid Compute

| On Device | Smartphone |
|-----------|------------|
| SLAM, Navigation, Object Recognition, Accessibility | Large model inference, Long-term memory, Heavy scene analysis |

**Target NPU:** 10–20 TOPS

### Gen 3 — Fully Autonomous Spatial Computer

Runs semantic world model, local multimodal AI, agent runtime, and spatial operating system. No smartphone required.

**Target Compute:** 40–100 TOPS

---

## Sensor Stack

| Sensor | Function | Target Spec |
|--------|----------|-------------|
| **Color LiDAR** | Depth, shape, spatial mapping | 0.1–50m range, 60Hz, 120° FOV |
| **Eye Tracking** | User intent, interface control | 240Hz |
| **IMU** | Head tracking, motion estimation | Accel + Gyro + Mag |
| **Privacy Camera** (optional) | OCR, text reading, explicit requests | Disabled by default, no retention |

---

## Semantic World Model

**Traditional systems store:** Images

**Sentinel stores:**
```
Chair  |  Table  |  Door  |  Plant  |  Person  |  Vehicle
```
...along with distance, orientation, and spatial relationships.

```
Chair beside table
Person standing near doorway
Dog under table
```

**Raw sensor data is discarded.**

---

## Privacy Architecture

| Tier | Guarantee |
|------|-----------|
| Tier 1 | No image storage |
| Tier 2 | No facial recognition |
| Tier 3 | No biometric profiles |
| Tier 4 | Ephemeral point cloud retention (<100ms) |
| Tier 5 | Semantic-only memory |
| Tier 6 | User privacy audit logs |
| Tier 7 | Hardware privacy indicators |

---

## AI Capabilities

- **Navigation** — Indoor and outdoor
- **Object Awareness** — Furniture, doors, appliances, vehicles, pets
- **Accessibility Narration** — *"Open doorway ahead."* / *"Three seats available."*
- **Spatial Memory** — *"Where are my keys?"*
- **Contextual Assistance** — *"Your laptop is still in the conference room."*

### Human Recognition Policy

| Allowed | Not Allowed |
|---------|-------------|
| Human present, direction, distance, motion | Identity, race, gender, age, emotion |

*(Unless explicitly enabled by user)*

---

## Hardware Requirements

| Spec | Gen 1 | Gen 2 | Gen 3 |
|------|-------|-------|-------|
| Weight | <65g | <75g | TBD |
| Battery | 16–24h | 12–16h | 10–14h |

**Connectivity:** WiFi, Bluetooth, UWB (optional: 5G)

**Display:** Waveguide AR — 1920×1080/eye, 90Hz, 3000+ nits, prescription support

---

## Operating System — SentinelOS

Subsystems:
- Sensor Manager
- Privacy Engine
- World Model Engine
- Agent Runtime
- Display Runtime

### Developer Platform

| API Type | Access |
|----------|--------|
| **Spatial APIs** | Nearby objects, room layouts, navigation graphs |
| **Context APIs** | User activity, environment type |
| **Agent APIs** | Semantic reasoning, spatial memory, AR overlays |

*Raw sensor streams unavailable to developers.*

---

## Security

- Secure boot
- Signed firmware
- Encrypted storage
- Trusted execution environment
- Hardware root of trust

---

## Business Model

| Stream | Pricing |
|--------|---------|
| **Hardware** | $799–$1,299 retail |
| **Software** | Future subscription: AI memory, cloud reasoning, fleet management |

### Manufacturing Targets

**Initial BOM Goal:** ~$425

| Component | Cost |
|-----------|------|
| Display | $120 |
| LiDAR | $90 |
| Battery | $25 |
| Electronics | $40 |
| Assembly | $30 |
| Other | $120 |

---

## Competitive Positioning

| Current AR Products | Sentinel |
|---------------------|----------|
| Visual capture | Environmental understanding |
| Media creation | Privacy |
| | Trust |
| | Accessibility |

---

## Strategic Moats

- Privacy-Preserving Spatial Computing
- Semantic-Only World Models
- Ephemeral Point Cloud Processing
- Geometry-First AR Operating Systems
- Privacy-Aware Spatial APIs

---

## Go-To-Market

| Phase | Focus | Users |
|-------|-------|-------|
| **Phase 1** | Accessibility | Visually impaired users |
| **Phase 2** | Enterprise | Warehouses, field service, industrial |
| **Phase 3** | Consumer | General-purpose AR assistant |

---

## Research Workstreams

| # | Workstream | Status |
|---|-----------|--------|
| 1 | Market Research | Open |
| 2 | Competitive Intelligence | Open |
| 3 | Hardware Architecture | Open |
| 4 | Privacy Architecture | Open |
| 5 | AI Architecture | Open |
| 6 | Economics | Open |
| 7 | Patent Strategy | Open |
| 8 | Founder Narrative | Open |
| 9 | Go To Market | Open |
| 10 | Investor Deck | Open |

---

## Long-Term Vision

**Sentinel becomes an ambient intelligence layer for the physical world.**

Instead of recording reality, it understands reality.

The platform augments human perception while preserving privacy, digity, and autonomy for everyone around it.
