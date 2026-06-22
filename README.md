# 🛡️ Project Sentinel

**Privacy-Preserving Semantic AR Glasses**

> *"Instead of recording reality, it understands reality."*

---

## The Problem

Every major AR company is building cameras for people's faces. Society will increasingly push back against this.

## Our Thesis

The winning AR platform will:
- **Understand** the world
- **Assist** the user  
- **Preserve** privacy
- **Maintain** social acceptability

## How It Works

Sentinel uses **Color LiDAR + local AI** instead of cameras:

| Cameras See | LiDAR Sees |
|-------------|------------|
| Faces, text, screens, license plates | Geometry, distance, shape, motion |
| Personally identifiable information | Spatial relationships only |

**We store meaning, not images.**

---

## Repository Structure

```
projectVision/
├── PRD.md              # Full product requirements document
├── README.md           # This file
├── docs/               # Research, architecture deep-dives
├── firmware/           # Embedded software (future)
├── sentinel-os/        # OS development (future)
├── tools/              # Developer tools, simulators (future)
└── .github/            # Issue templates, workflows
```

## Tech Stack (Planned)

- **Sensing:** Color LiDAR, IMU, Eye Tracking
- **Compute:** Gen 1 smartphone-tethered → Gen 3 fully autonomous
- **OS:** SentinelOS (Sensor Manager, Privacy Engine, World Model, Agent Runtime)
- **AI:** Local semantic reasoning, spatial memory, AR overlays

## Privacy By Design

Seven-tier privacy architecture:
1. No image storage
2. No facial recognition
3. No biometric profiles
4. Ephemeral point clouds (<100ms)
5. Semantic-only memory
6. User audit logs
7. Hardware privacy indicators

## Business Model

- **Hardware:** $799–$1,299
- **Software:** Future subscription (AI memory, cloud reasoning, fleet management)
- **Target BOM:** ~$425

## Go-To-Market

1. **Phase 1:** Accessibility (visually impaired)
2. **Phase 2:** Enterprise (warehouses, field service)
3. **Phase 3:** Consumer (general-purpose AR)

---

## Status

Currently in **pre-seed exploration**. See [PRD.md](PRD.md) for the full product requirements.

### Open Research Workstreams

- [ ] Market Research
- [ ] Competitive Intelligence
- [ ] Hardware Architecture
- [ ] Privacy Architecture
- [ ] AI Architecture
- [ ] Economics
- [ ] Patent Strategy
- [ ] Founder Narrative
- [ ] Go To Market
- [ ] Investor Deck

---

*Built with privacy as a feature, not an afterthought.*
