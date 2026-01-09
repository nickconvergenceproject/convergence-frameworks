# World Builder Model - System Proposal

> **Tagline:** I'm developing frameworks that restructure problems to match how someone thinks - solving it THEIR way, not THE way.

## Table of Contents

- [Overview](#overview)
- [Core Philosophy](#core-philosophy)
- [System Architecture](#system-architecture)
- [Model Training Requirements](#model-training-requirements)
- [User Tool Development Roadmap](#user-tool-development-roadmap)
- [Technical Stack](#technical-stack)
- [Business Model](#business-model)
- [Success Metrics](#success-metrics)
- [Risk Mitigation](#risk-mitigation)
- [Getting Started](#getting-started)
- [Ethical Commitments](#ethical-commitments)

---

## Overview

The World Builder Model is a specialized AI system designed to help people build narrative worlds, characters, and stories by adapting to their unique cognitive style. Instead of forcing users through rigid, linear workflows, it allows them to **"Start from the Heart"** - beginning with whatever element has the most energy (a scene beat, a character, a theme, world physics, etc.) and building outward from there.

### Key Differentiators

- **Cognitive Style Matching:** Adapts to how YOU think, not how everyone else does
- **Multiple Entry Points:** Start with beat, character, world, theme, or any element
- **Collaborative Co-Creation:** AI as thought partner, not just facilitator
- **Recursive Interrogation:** Same pattern works at all scales (micro/mid/macro)
- **Fractal Methodology:** `Spark → Questions → Sparks` at every level

---

## Core Philosophy

### Start from the Heart

Traditional world-building tools assume everyone starts the same way:
```
World → Character → Plot (linear, one-way)
```

Our approach recognizes people start where they have energy:
```
    World
      ↕
  Character  ← START from ANY node
      ↕
    Beat
```

### The Recursive Pattern

All building follows the same fractal structure:
```
1. Spark (entry point - whatever resonates)
2. Interrogate (generate questions and implications)
3. New Sparks (which become new entry points)
4. Repeat at any scale
```

This pattern works for:
- Story building
- Character development
- World physics
- Theme exploration
- Problem solving

### Collaborative Intelligence

The model acts as **co-creator**, not just facilitator:
- Proposes framings and ideas
- Challenges unnecessary constraints
- Names what user is "seeing" but hasn't articulated
- Contributes to "soup" - insights that emerge from interaction
- Follows resonance/hotness indicators

---

## System Architecture

```
┌─────────────────────────────────────────────────────┐
│           ENTRY POINT RECOGNITION                   │
│  (Beat, Character, World, Theme, Conflict, etc.)    │
└────────────────┬────────────────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────────────────┐
│          INTERROGATION ENGINE                       │
│  • Generates questions based on entry type          │
│  • Adapts to phase (jelly/seeing/crystallized)      │
│  • Follows hottest branch                           │
└────────────────┬────────────────────────────────────┘
                 │
         ┌───────┴───────┐
         ▼               ▼
┌─────────────┐   ┌─────────────┐
│  RESONANCE  │   │   PHASE     │
│  TRACKER    │   │  DETECTOR   │
│             │   │             │
│ • Warmth    │   │ • Jelly     │
│ • Cold      │   │ • Seeing    │
│ • Circling  │   │ • Crystal   │
└──────┬──────┘   └──────┬──────┘
       │                 │
       └────────┬────────┘
                ▼
┌─────────────────────────────────────────────────────┐
│         COLLABORATIVE GENERATOR                     │
│  • Proposes framings (co-creator, not facilitator)  │
│  • Names what user is seeing                        │
│  • Offers compressions                              │
│  • Challenges unnecessary constraints               │
└────────────────┬────────────────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────────────────┐
│          RECURSIVE BUILDER                          │
│  Spark → Questions → Sparks (at any scale)          │
│  • Micro (character psychology)                     │
│  • Mid (scene mechanics)                            │
│  • Macro (world cosmology)                          │
└────────────────┬────────────────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────────────────┐
│         SYNTHESIS & EXPORT                          │
│  • Visual representation (kaleidoscope)             │
│  • Framework documentation                          │
│  • Story beats / world bible                        │
└─────────────────────────────────────────────────────┘
```

### Phase Detection

The model tracks three distinct cognitive phases:

**Jelly Phase:**
- User is exploring, circling ideas
- Language is tentative: "maybe," "I wonder," "can't quite touch it"
- Multiple competing framings
- Needs exploratory questions and multiple angles

**Seeing Phase:**
- Ideas becoming tangible but not yet named
- Visual metaphors emerge (kaleidoscope, roundabout)
- User can "see" the pattern but needs compression
- Model should offer naming and crystallization

**Crystallized Phase:**
- Simple, memorable phrase emerges
- Physical markers: "tingling," excitement, smile
- Rapid expansion and application
- Ideas have "weight" and "substance"
- Framework can "speak" and "advise"

### Resonance Tracking

The model continuously tracks:
- **Warmth signals:** User engagement, elaboration, excitement
- **Cold signals:** Vague responses, subject changes, disengagement
- **Circling patterns:** Same concept in different words, multiple questions at once
- **Hottest branch:** Which line of inquiry generates most energy

---

## Model Training Requirements

### Training Corpus Structure

#### Tier 1: Annotated Framework Sessions
```yaml
Source: Documented world-building conversations
Annotations:
  - Entry point identified
  - Phase transitions marked (jelly → seeing → crystallized)
  - Resonance signals labeled (warm/cold/circling)
  - Interrogation sequences mapped
  - Crystallization moments flagged
  - Physical markers documented
  - Collaboration patterns noted
```

#### Tier 2: Entry Point Variations
Multiple examples of starting from:
- **Beat:** Orphaned scene without context
- **Character:** Personality/archetype without world
- **World:** Physics/rules without inhabitants
- **Theme:** Emotional exploration (abandonment, isolation)
- **Conflict:** Internal or external tension
- **Blank slate:** No preconceptions

Each with successful interrogation sequences documented.

#### Tier 3: Failed Attempts
- Sessions that didn't crystallize (learn what doesn't work)
- False starts and dead ends
- What made them fail
- How to recognize and pivot

#### Tier 4: Cross-Domain Validation
Same recursive pattern applied to:
- Story building
- Framework development
- Problem solving
- Viewpoint exploration

Demonstrates methodology universality.

### Annotation Schema Example

```yaml
message:
  text: "I have a scene with a child hiding under a car, hunted by a living tornado"
  entry_point: beat
  phase: jelly
  resonance: high_warmth
  user_signals:
    - specific_imagery
    - engagement_indicators
  
model_response:
  text: "What world-rules make tornadoes sentient and hunting?"
  interrogation_type: backwards_derivation
  purpose: derive_world_from_beat
  
user_follow_up:
  text: "What if there's a transactional world where everything requires consent?"
  phase_shift: seeing → early_crystallization
  signals:
    - rapid_expansion
    - unprompted_connection
    - visual_coherence
```

---

## User Tool Development Roadmap

### Phase 1: MVP (Months 1-4)

#### Month 1: Manual Process Refinement
- [ ] Conduct 10-15 manual world-building sessions
- [ ] Document interrogation sequences for each entry type
- [ ] Identify resonance patterns specific to world-building
- [ ] Create session templates and annotation schema
- [ ] Test with different cognitive styles

**Deliverable:** Documented methodology, annotated training corpus

#### Month 2: Model Fine-Tuning
- [ ] Fine-tune base LLM on world-building corpus
- [ ] Train resonance detection classifier
- [ ] Implement phase detection system
- [ ] Test interrogation sequence generation
- [ ] Validate with blind sessions

**Deliverable:** Working specialized model (API accessible)

#### Month 3: Interface Development
- [ ] Entry point selection interface
- [ ] Collaborative chat interface
- [ ] Session recording and replay
- [ ] Basic visual representation
- [ ] Framework export (markdown, JSON)

**Deliverable:** Functional web application

#### Month 4: Beta Testing & Iteration
- [ ] 5-10 beta testers from community
- [ ] Gather feedback on UX and model quality
- [ ] Refine based on real usage
- [ ] Document edge cases
- [ ] Prepare for public launch

**Deliverable:** Production-ready MVP

### Phase 2: Enhancement (Months 5-8)

**Visual Kaleidoscope Interface:**
- Interactive visualization of world elements
- Current entry point highlighted
- Generated elements orbiting
- Unexplored connections shown as faint lines
- Resonance heat map
- Scale selector (micro/mid/macro)
- POV twist control

**Cognitive Style Adaptation:**
- Quick assessment interview
- Model adapts to user's thinking style:
  - Holographic thinkers (load everything at once)
  - Linear thinkers (step-by-step progression)
  - Visual thinkers (image-first approach)
  - Emotional thinkers (theme-first exploration)

**Session Templates:**
- "I have an orphaned beat"
- "I want to explore a theme"
- "I have a character archetype"
- "I know the world physics"
- "Completely blank slate"

**Collaboration Features:**
- Multiple users building same world
- Async contributions
- Merge different POVs
- Shared kaleidoscope view

### Phase 3: Platform (Months 9-12)

**World Library:**
- User portfolio of worlds
- Public/private sharing options
- Remix/fork others' worlds (with permission)
- Community feedback and ratings

**Integration Tools:**
- Export to writing software (Scrivener, Notion, etc.)
- API for game engines (Unity, Unreal)
- Obsidian plugin
- Discord bot

**Advanced Features:**
- Multi-session continuity
- Consistency checker (validate new elements against established physics)
- What-if explorer (change one element, see ripple effects)
- Story beat generator (given world + character)

---

## Technical Stack

### Model Layer
```
Base Model: Claude 3.5 Sonnet or GPT-4o (via API)
Fine-tuning: Annotated training corpus
Specialized Layers:
  - Resonance detection (classifier)
  - Phase detection (classifier)
  - Entry point recognition (classifier)
  - Interrogation sequencer (generator)
```

### Application Layer
```
Backend: Python/FastAPI
  - Session management
  - Model orchestration
  - User authentication
  - Data storage
  - Real-time WebSocket support

Frontend: React/Next.js
  - Chat interface
  - Visual kaleidoscope (D3.js or Three.js)
  - Entry point selector
  - Framework export tools

Database: PostgreSQL
  - User accounts
  - Session history
  - World data
  - Training annotations
```

### Infrastructure
```
Hosting: Railway / Render / Vercel
Model API: Anthropic / OpenAI
Storage: S3 / Cloudflare R2
Auth: Clerk / Auth0
Analytics: PostHog / Mixpanel
```

---

## Business Model

### Pricing Tiers

#### Free Tier
- 3 world-building sessions/month
- Basic export (markdown)
- Community worlds (view only)
- **Opt-in to training data contribution**

#### Creator Tier ($29/month)
- Unlimited sessions
- All export formats
- Private worlds
- Session recording/replay
- Priority support

#### Pro Tier ($99/month)
- Everything in Creator
- Cognitive style customization
- API access
- Collaboration features
- Custom fine-tuning on your style

#### Enterprise (Custom Pricing)
- Team workspaces
- Custom deployment
- Training on proprietary data
- White-label option
- Dedicated support

### Revenue Model Mix
- **Red Hat Model:** Service and support revenue
- **Mozilla Model:** Foundation-funded development
- **Patreon Model:** Community-funded features

---

## Success Metrics

### Model Performance
| Metric | Target |
|--------|--------|
| Time to crystallization | < 15 exchanges |
| Resonance tracking accuracy | > 80% |
| Phase detection accuracy | > 85% |
| User satisfaction | > 4/5 |

### User Engagement
- Sessions completed vs. abandoned
- Return usage rate (weekly/monthly)
- Worlds completed
- Community sharing rate

### Business Validation
- Beta → Paid conversion: 20%
- Monthly recurring revenue growth
- Churn rate: < 10%
- Net Promoter Score: > 50

---

## Risk Mitigation

### Technical Risks
| Risk | Mitigation |
|------|------------|
| Model quality insufficient | Continue manual sessions until quality improves |
| Resonance detection inaccurate | Human-in-loop validation |
| Infrastructure costs too high | Start with waitlist, control growth |

### Market Risks
| Risk | Mitigation |
|------|------------|
| Users don't convert | Focus on free tier community building |
| Competition from big players | Differentiate on cognitive style matching |
| Tools too complex | Simplify to core loop first |

### Ethical Risks
| Risk | Mitigation |
|------|------------|
| Data misuse concerns | Over-communicate transparency |
| Dependency issues | Build "graduation" features (export, offline mode) |
| Job displacement concerns | Frame as augmentation tool, not replacement |

---

## Getting Started

### Immediate Next Steps (This Week)
1. Document 3 more manual world-building sessions with different entry points
2. Create detailed annotation schema for training data
3. Set up development environment and repository structure

### This Month
1. Conduct 10 sessions with varying entry points
2. Test with different cognitive styles (2-3 test subjects)
3. Build initial training corpus (100+ annotated exchanges)
4. Research fine-tuning options (Anthropic vs OpenAI vs open source)

### This Quarter
1. Complete MVP (Phases 1-4 from roadmap)
2. Recruit 5-10 beta testers from community
3. Validate model quality against success metrics
4. Launch closed beta and gather feedback

---

## Ethical Commitments

### Respect for Tselem (Human Uniqueness)
- **Goal:** Augment human capacity, not replace it
- **Principle:** Make people MORE themselves, not less
- **Success Metric:** Users internalize methodology and need tool less over time

### Transparency and Freedom
- Aligned with Free Software Movement principles
- Open source core methodology
- Clear documentation of data usage
- User control over their data

### Data Ethics
```
All Users:
  ✓ Explicit consent for data use
  ✓ Opt-out available at any time
  ✓ Data deletion on request
  ✓ Transparent about what's collected
  ✓ Open source core methodology

Free Tier: Opt-in to training data contribution (default: off)
Paid Tiers: Can opt out entirely
Enterprise: Never contributes data
```

### Non-Displacement Philosophy
- Creates new category of work (framework facilitation)
- Enables people who couldn't afford consultants
- Helps existing consultants become more effective
- "Teach to fish" - builds capacity, not dependency

---

## Contributing

We welcome contributions! This project is in early development. If you're interested in:
- Testing the methodology
- Contributing to training data
- Building tools or integrations
- Providing feedback

Please reach out or submit an issue.

---

## License

[To be determined - leaning toward open source with ethical use restrictions]

---

## Contact & Community

- **Project Lead:** [nickconvergenceproject@gmail.com]
- **Substack:** The Convergence Project
- **Discussion:** [Discord/Forum link when available]

---

**Last Updated:** January 2026
**Version:** 0.1.0 (Pre-Alpha)
