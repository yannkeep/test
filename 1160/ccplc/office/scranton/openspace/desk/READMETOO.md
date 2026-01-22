# NLnet NGI Zero Commons Fund Application

## CivicARG — Open Civic Simulation Engine

---

## 1. ABSTRACT (250 words max)

**CivicARG** is an open source JavaScript/HTML framework for building interactive civic education experiences through Alternate Reality Games (ARGs).

Democratic systems are increasingly complex, and citizens feel disconnected from institutions they don't understand. Traditional civic education fails to convey systemic issues like bureaucratic capture, particracy, or institutional dysfunction.

CivicARG addresses this by providing a **reusable, country-agnostic engine** that transforms dry political science into engaging narrative games. Players interact with satirical-realistic NPCs (bureaucrats, officials, activists), complete missions revealing systemic issues, and discover easter eggs rewarding curiosity.

The framework consists of:
- **Dialogue Engine**: Branching conversations with choices affecting player state
- **Mission Engine**: Progressive quests with prerequisites and rewards
- **Profile System**: Civic score, political "pillar" assignment, awareness stats
- **Easter Egg System**: Hidden content revealed through exploration
- **Configuration Schema**: JSON-based country definitions (institutions, NPCs, missions)

All components are **fully configurable** — any country can adapt the engine to teach their specific political system. The Belgium demo configuration serves as proof-of-concept, covering pilarization, particracy, and federal complexity.

**Key deliverables:**
- Core engine (vanilla JS, no dependencies)
- Visual dialogue/mission editor
- 3 country configurations (Belgium, France, EU institutions)
- Documentation and contributor guidelines
- Accessibility compliance (WCAG 2.1 AA)

CivicARG empowers educators, journalists, and civic organizations to create engaging democratic literacy tools — without reinventing the wheel for each country.

---

## 2. HAVE YOU BEEN INVOLVED WITH NLNET BEFORE?

No.

---

## 3. REQUESTED AMOUNT

**€45,000**

---

## 4. PROJECT DESCRIPTION

### 4.1 Problem Statement

Civic engagement across Europe is declining. According to Eurobarometer, only 49% of EU citizens feel their voice counts, and trust in national institutions averages just 35%. Young people are particularly disengaged — not because they don't care, but because they can't understand systems that seem designed to be opaque.

Traditional civic education approaches (textbooks, lectures, websites) fail for several reasons:
- **Abstract**: Explaining "consociational democracy" doesn't convey lived experience
- **Boring**: Passive consumption doesn't create lasting understanding
- **Disconnected**: Generic content doesn't relate to specific national contexts
- **One-way**: No feedback loop showing why systems produce certain outcomes

Meanwhile, evidence from game-based learning research shows that interactive narratives significantly improve comprehension and retention of complex systems.

### 4.2 Proposed Solution

CivicARG is a **framework**, not just a game. It provides the building blocks for anyone to create civic simulation experiences:

**Technical Components:**
1. **Core Engine** (JavaScript ES6+, vanilla, no dependencies)
   - State management (player profile, progress, flags)
   - Event system (dialogue choices → effects → revelations)
   - Save/load (localStorage, export/import)
   - Theming (CSS custom properties)

2. **Dialogue Engine**
   - NPC definitions (name, personality, dialogue trees)
   - Branching paths with conditions
   - Effects on player stats
   - Typing animation for immersion

3. **Mission Engine**
   - Quest definitions with steps
   - Prerequisites and dependencies
   - Progress tracking
   - Rewards (score, unlocks, revelations)
   - "Impossible missions" for satirical effect

4. **Easter Egg Engine**
   - Console messages
   - Konami code activation
   - Trigger-based content revelation
   - Hidden news/documents

5. **Configuration Schema**
   - JSON-based country definition
   - Pillars/political families
   - Institutions
   - NPCs and dialogues
   - Missions
   - Localization (i18n)

**Content Components:**
- Belgium configuration (proof of concept, included)
- France configuration (deliverable)
- EU institutions configuration (deliverable)

**Tooling Components:**
- Visual dialogue editor (web-based)
- Mission graph visualizer
- Config validator
- Documentation generator

### 4.3 Innovation

CivicARG is novel in several ways:

1. **Framework approach**: Unlike one-off civic games, CivicARG is designed for reuse. The Belgium-specific content demonstrates the framework, but the engine works for any democracy.

2. **Satirical-realistic methodology**: We use humor as a cognitive tool. By exaggerating real dysfunctions to the point of absurdity, we make them visible and memorable. This approach is grounded in political satire traditions (Swift, Havel) and learning research.

3. **Easter egg pedagogy**: Hidden content rewards curiosity and critical thinking. Players who dig deeper learn more — modeling the skills needed for informed citizenship.

4. **Pillar-based profiling**: The system assigns players to "political pillars" based on their choices, making abstract ideological positions concrete and personal.

### 4.4 Sustainability

Post-funding sustainability is built into the design:

1. **Low maintenance**: No server required, static HTML/JS
2. **Community contributions**: Country configs can be contributed by local communities
3. **Educational adoption**: Free for schools and NGOs
4. **Commercial license**: Optional paid support/customization for governments or large organizations
5. **Foundation model**: Potential fiscal hosting by existing European digital commons organizations

### 4.5 European Dimension

CivicARG directly addresses EU priorities:
- **Digital citizenship**: Teaching citizens to navigate democratic systems
- **Media literacy**: Critical thinking about information and institutions
- **European identity**: EU institutions configuration creates shared understanding
- **Multilingualism**: i18n support for all EU languages
- **Open source commons**: All code under EUPL-1.2

The project originates in Belgium (Brussels), involves contributors from France and Germany, and targets EU-wide deployment.

---

## 5. MILESTONES

### M1: Core Engine (Month 1-2) — €8,000
- [ ] Dialogue engine with branching and effects
- [ ] Mission engine with prerequisites
- [ ] Player profile system
- [ ] Easter egg engine
- [ ] Save/load functionality
- [ ] Basic theming support
- **Deliverable**: Working single-file engine with Belgium demo

### M2: Belgium Configuration (Month 2-3) — €7,000
- [ ] Complete pillar definitions (5 pillars)
- [ ] NPC dialogues (3 NPCs, 50+ dialogue nodes)
- [ ] Mission set (5 missions)
- [ ] News feed content (20+ items)
- [ ] Easter eggs (10+)
- [ ] French localization
- **Deliverable**: Playable Belgium demo

### M3: Visual Editor (Month 3-4) — €10,000
- [ ] Dialogue editor (node-based interface)
- [ ] Mission graph visualizer
- [ ] Config validator
- [ ] Preview mode
- [ ] Export functionality
- **Deliverable**: Web-based editing tool

### M4: France Configuration (Month 4-5) — €7,000
- [ ] French political pillar definitions
- [ ] NPC dialogues adapted to French context
- [ ] Mission set covering French specificities
- [ ] Full French localization
- **Deliverable**: Playable France demo

### M5: EU Configuration (Month 5-6) — €7,000
- [ ] EU institutions pillar definitions
- [ ] NPC dialogues (Commission, Parliament, Council)
- [ ] Mission set covering EU decision-making
- [ ] English localization (primary)
- **Deliverable**: Playable EU demo

### M6: Documentation & Accessibility (Month 6) — €6,000
- [ ] Comprehensive documentation
- [ ] WCAG 2.1 AA compliance audit
- [ ] Contributor guidelines
- [ ] Example configuration template
- [ ] Video tutorials
- **Deliverable**: Publication-ready project

---

## 6. BUDGET BREAKDOWN

| Category | Amount | % |
|----------|--------|---|
| Core development | €18,000 | 40% |
| Content creation | €14,000 | 31% |
| Tooling | €10,000 | 22% |
| Documentation & QA | €3,000 | 7% |
| **Total** | **€45,000** | 100% |

All amounts are for human labor (no hardware, hosting, or licenses needed).

---

## 7. TEAM

**Lead Developer**: [Your Name]
- Background in civic tech and political science
- Experience with web development and game design
- Based in Brussels, Belgium

**Contributors** (part-time):
- Political scientist (content validation)
- UX designer (accessibility)
- Translator (FR/NL/DE)

---

## 8. OPEN SOURCE COMMITMENT

All deliverables will be released under **EUPL-1.2** (European Union Public License), with a permissive **MIT** dual-license option for maximum compatibility.

Repository: [GitHub/GitLab URL - to be created]

The project will follow open source best practices:
- Public issue tracker
- Contribution guidelines
- Code of conduct
- Semantic versioning
- Automated testing

---

## 9. COMPARABLE PROJECTS

| Project | Comparison |
|---------|------------|
| **Democracy 4** (game) | Commercial, not open source, not educational |
| **iCivics** (US) | US-specific, not framework-based, Flash legacy |
| **Kahoot** | Quiz-based, not narrative/simulation |
| **Twine** | General interactive fiction, not civic-specific |

CivicARG fills a gap: **no open source, reusable, narrative-based civic education framework exists**.

---

## 10. CONTACT

**Name**: [Your Name]
**Email**: [your.email@example.org]
**Location**: Brussels, Belgium
**Languages**: French, English, Dutch

---

*Submitted to NGI Zero Commons Fund, [Date]*
