# CivicARG Engine

**Open Source Civic Simulation Framework**

[![License: EUPL-1.2](https://img.shields.io/badge/License-EUPL--1.2-blue.svg)](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 What is CivicARG?

CivicARG is an **open source JavaScript/HTML framework** for building interactive civic education experiences through Alternate Reality Games (ARGs). It enables educators, journalists, and civic organizations to create engaging simulations that teach citizens about democratic systems, institutions, and political dynamics.

### The Problem

- Civic education is often boring, abstract, and disconnected from lived reality
- Citizens feel powerless and disengaged from complex political systems  
- Traditional teaching methods fail to convey systemic issues (bureaucracy, particracy, institutional capture)
- Each country reinvents educational materials from scratch

### The Solution

CivicARG provides a **reusable, configurable engine** that any country can adapt:

- **Narrative-driven learning** through dialogues with NPCs (bureaucrats, officials, activists)
- **Mission-based progression** revealing systemic issues step by step
- **Satirical-realistic approach** making critique accessible through humor
- **Easter eggs and revelations** rewarding curious players with deeper insights
- **Fully localizable** with i18n support for any language

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                      CivicARG Engine                            │
├─────────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐             │
│  │   Country   │  │  Dialogue   │  │   Mission   │             │
│  │   Config    │  │   Engine    │  │   Engine    │             │
│  │   (JSON)    │  │             │  │             │             │
│  └─────────────┘  └─────────────┘  └─────────────┘             │
│         │                │                │                     │
│  ┌──────┴────────────────┴────────────────┴──────┐             │
│  │              Core State Manager                │             │
│  │   (player profile, progress, achievements)     │             │
│  └──────┬────────────────┬────────────────┬──────┘             │
│         │                │                │                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐             │
│  │    Feed     │  │ Easter Egg  │  │     UI      │             │
│  │   Engine    │  │   Engine    │  │  Renderer   │             │
│  └─────────────┘  └─────────────┘  └─────────────┘             │
└─────────────────────────────────────────────────────────────────┘
```

### Core Components

| Component | Purpose |
|-----------|---------|
| **CountryConfig** | JSON schema defining country-specific elements (pillars, institutions, NPCs, missions) |
| **DialogueEngine** | Branching conversation system with choices, effects, and typing animations |
| **MissionEngine** | Quest/task management with prerequisites, progress tracking, and rewards |
| **FeedEngine** | News/event system with hidden items revealed by player actions |
| **EasterEggEngine** | Hidden content management (console messages, Konami codes, secret triggers) |
| **ProfileEngine** | Player state (civic score, pillar assignment, stats, flags) |

---

## 🌍 Adaptability

### Supported Configurations

The framework is designed to be **country-agnostic**. All political/cultural specifics are defined in a JSON configuration:

```javascript
const COUNTRY_CONFIG = {
  id: "belgium",
  name: "Kingdom of Belgium",
  emoji: "🇧🇪",
  motto: "L'union fait la force",
  languages: ["fr", "nl", "de"],
  
  // Political pillars (adapt to any system)
  pillars: [
    { id: "socialist", name: "Socialist Pillar", color: "#e63946", ... },
    { id: "christian", name: "Christian-Democrat Pillar", color: "#f4a261", ... },
    // ...
  ],
  
  // NPCs and dialogues
  npcs: { ... },
  
  // Missions
  missions: [ ... ],
  
  // Easter eggs
  easterEggs: [ ... ],
  
  // Translations
  i18n: { ... }
}
```

### Example Use Cases

| Country | Theme | Pillars |
|---------|-------|---------|
| **Belgium** | Pilarization, particracy, federal complexity | Socialist, Christian, Liberal, Ecological, Nationalist |
| **France** | Centralization, technocracy, social movements | Gaullist, Socialist, Centrist, Ecological, Populist |
| **Germany** | Federal system, coalition politics | CDU/CSU, SPD, Green, Liberal, AfD |
| **Netherlands** | Consensus democracy, verzuiling | Similar to Belgium |
| **Poland** | Democratic backsliding, EU tensions | PiS, PO, Left, Konfederacja |
| **EU** | Brussels bubble, democratic deficit | Federalist, Sovereignist, Technocratic |

---

## 🎮 Features

### Dialogue System
- Branching conversations with multiple NPCs
- Choices affecting player stats and story progression
- Typing animation for immersive experience
- Conditional dialogue paths based on player state

### Mission System
- Progressive unlock system
- Prerequisites and dependencies
- Impossible missions (satirical element)
- Rewards (civic score, unlocks, revelations)

### Player Profile
- **Civic Score**: Overall engagement metric
- **Pillar Assignment**: Political positioning
- **Stats**: Compliance, Awareness, Trust, Knowledge, Suspicion
- **Flags**: Track story choices and discoveries

### Easter Eggs
- Console messages for developers
- Konami code for debug mode
- Hidden news items revealed by awareness level
- Redacted text revealed on hover
- Secret dialogues and endings

### Visual Design
- Themeable via CSS custom properties
- Particle system for ambiance
- Glassmorphism UI
- Dark/light mode support
- Accessibility compliant (WCAG 2.1 AA)

---

## 📦 Technical Specifications

### Requirements
- Modern browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- JavaScript ES6+
- No external dependencies (vanilla JS)
- Single HTML file deployment possible

### Size
- ~50KB uncompressed (single file)
- ~15KB gzipped

### Performance
- 60 FPS animations
- Lazy loading for heavy content
- LocalStorage for save games
- Offline-capable (PWA-ready)

---

## 🚀 Roadmap

### Phase 1: Core Engine (Current)
- [x] Dialogue system
- [x] Mission system
- [x] Player profile
- [x] Easter eggs
- [x] Belgium demo config

### Phase 2: Tooling
- [ ] Visual dialogue editor
- [ ] Mission graph visualizer
- [ ] Config validator
- [ ] Translation workflow

### Phase 3: Extensions
- [ ] Multiplayer/social features
- [ ] Community mission sharing
- [ ] Analytics dashboard
- [ ] API for external integrations

### Phase 4: Content
- [ ] France configuration
- [ ] Germany configuration
- [ ] EU institutions configuration
- [ ] Community contributions

---

## 📄 License

Dual-licensed under:
- **EUPL-1.2** (European Union Public License)
- **MIT License**

Choose the license that best fits your needs.

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Priority Areas
1. New country configurations
2. Translations (i18n)
3. Accessibility improvements
4. Documentation
5. Visual editor tooling

---

## 📬 Contact

- **Project Lead**: [Your Name]
- **Email**: civicarg@example.org
- **Matrix**: #civicarg:matrix.org
- **Mastodon**: @civicarg@fosstodon.org

---

## 🙏 Acknowledgments

This project is inspired by:
- Belgian political satire traditions
- Serious games research
- Civic tech movement
- Open source communities

---

*CivicARG: Making democracy understandable, one sarcastic bureaucrat at a time.*
