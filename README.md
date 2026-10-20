# Truinorva TRIZ — A Comprehensive TRIZ Plugin for Claude

> **TRIZ for Innovation, R&D, and Product Teams.** Move from random brainstorming to structured, contradiction-driven problem solving. 26 model-invoked skills covering the full TRIZ toolkit — function analysis, contradiction resolution, root-cause and root-conflict analysis, resource analysis, ideality, system operator, trimming, patent analysis, and more.

Maintained by **[Truinorva](https://truinorva.de)** — innovation consulting and training combining TRIZ methodology with AI-enabled R&D workflows.

---

## Why this plugin?

Most "ideation" tools generate variations of the same idea. **TRIZ generates the right idea** by exposing the contradiction at the heart of the problem and resolving it with patterns extracted from millions of patents. This plugin packages the methods Truinorva uses with industrial R&D and product teams into model-invoked Claude skills — Claude picks the right tool for the right step automatically.

- **For R&D engineers** — function models, contradictions, trimming, patent analysis
- **For product managers** — MPVs, ideality, system evolution
- **For innovation consultants & trainers** — a portable TRIZ toolkit for client work
- **For non-technical teams** — Business-TRIZ skills for HR, service, retail, and operations

---

## Installation

Once listed in the official Anthropic plugin directory:

```bash
/plugin install truinorva-triz@claude-plugins-official
```

Or, while in review / for direct GitHub install:

```bash
/plugin marketplace add truinorva/truinorva-triz
/plugin install truinorva-triz
```

Skills are model-invoked — once installed, Claude automatically activates the relevant skill based on what you're working on. You can also call them by name (e.g. *"Use function-analysis on this system"*).

---

## Skills overview (26 total)

### 🧭 System Definition & Framing

| Skill | What it does |
|---|---|
| **system-description** | Mini-ISQ — guides you through a clear technical system and problem description via structured questions. The starting point for any TRIZ analysis. |
| **innovation-checklist** | Full Innovation Situation Questionnaire (ISQ / ISQ++) — captures responses, optional Excel export. |
| **system-operator** | 9 Boxes / 9 Screens — analyzes a technical system across past/present/future at Super-System, System, and Sub-System levels. Evolution-oriented or problem-oriented. |
| **business-msd** | Multi-Screen Diagram for business systems — 9 windows applied to organizational and market evolution. |
| **mpv-analysis** | PV / MPV Analysis — identifies Parameters of Value and Main Parameters of Value to focus innovation on what customers actually value. |

### 🔧 Function Analysis

| Skill | What it does |
|---|---|
| **function-analysis** | Classic TRIZ Function Analysis — Tool–Action–Object mapping, useful/harmful classification, function model. |
| **function-analysis-advanced** | Adds spatio-temporal dimensions (when/where) to surface timing and location mismatches. |
| **function-interaction-analysis** | Maps energy / matter / information flow between components. |
| **business-function-analysis** | Simplified Function Analysis for non-engineering domains (HR, education, healthcare, retail, hospitality). |

### 🔍 Cause & Conflict Analysis

| Skill | What it does |
|---|---|
| **root-cause-analysis** | Engineering RCA — scientific principles, physical parameters, actionable root causes. |
| **cause-effect-chain-analysis** | TRIZ CECA — traces causal chains from symptoms to root causes and emerging contradictions. |
| **root-conflict-analysis** | RCA+ / Grundkonfliktanalyse — models states that are *simultaneously* useful and harmful, formulates contradiction statements ready for inventive resolution. |
| **perception-mapping** | Surfaces stakeholder beliefs, builds Leads-To networks, exposes hidden contradictions in people-heavy or politically nuanced problems. |

### ⚔️ Contradiction Resolution

| Skill | What it does |
|---|---|
| **contradiction-solver** | The classic — Altshuller Matrix, Matrix 2003, and the 40 Inventive Principles for engineering contradictions. |
| **physical-contradictions** | Resolves physical contradictions (one parameter must take two opposing values) using the four separation principles: space, time, parts/whole, condition. |
| **76-standard-solutions** | Substance-Field Analysis (Su-Field) plus the 76 Standard Solutions in 5 classes — for harmful, insufficient, or missing interactions. |

### 💎 Resources & Ideality

| Skill | What it does |
|---|---|
| **resource-analysis** | All six TRIZ resource types (material, field, functional, informational, spatial, temporal — MATChEMIB). |
| **derivative-resources** | Finds *new* resources arising through combination, transformation, or reinterpretation of what's already in the system. |
| **ideality** | Drives a system toward its Ideal Final Result by reducing harm and increasing usefulness without adding cost. |

### 💡 Solution Generation

| Skill | What it does |
|---|---|
| **trimming** | Classic TRIZ Trimming with Rules A, B, C — eliminate components while preserving function. |
| **interactive-trimming** | Extended trimming with Rules A–E and X — covers external components, new markets, better alternatives. |
| **feature-transfer** | Combines advantages of competing or analogous systems. |
| **function-oriented-search** | FOS / MOS / Scientific Effects — finds how other industries or nature solve the same function (AskNature, Oxford Creativity, etc.). |
| **solutions-at-system-levels** | Business-TRIZ — generates ideas at Super-System and Sub-System levels. |
| **smart-little-people** | SLP method — overcomes psychological inertia by visualizing tiny agents inside the system. |

### 📄 Domain-Specific

| Skill | What it does |
|---|---|
| **patent-analyzer** | Reads patents and extracts engineering / physical contradictions, mapping problem parameters to TRIZ parameters via synonyms. |

---

## Suggested workflows

**New problem, no clear definition yet:**
`system-description` → `innovation-checklist` → `mpv-analysis`

**Mature system, hard to improve:**
`function-analysis` → `cause-effect-chain-analysis` → `root-conflict-analysis` → `contradiction-solver` / `physical-contradictions`

**System feels too complex:**
`function-analysis` → `trimming` (or `interactive-trimming`) → `ideality`

**Looking for inspiration outside your domain:**
`function-analysis` → `function-oriented-search` → `feature-transfer`

**Working with patents:**
`patent-analyzer` → `contradiction-solver` → `system-operator`

---

## Authoring & methodology

Skills are based on canonical TRIZ literature (Altshuller, Terninko/Zusman/Slotin, MATRIZ Body of Knowledge) and on Truinorva's training and consulting practice. German terminology follows Jens Träger's preferred MATRIZ Level-3+ conventions where applicable.

For background, see the related projects:
- 🛠 [`triz-prompt-engineering`](https://github.com/jenstraeger/triz-prompt-engineering) — XML-based TRIZ prompt templates (MIT license)

---

## License

MIT License — see [LICENSE](LICENSE).

Skills are provided "as is" for educational and professional use. They reflect TRIZ methodology as taught and practiced; results in any specific engineering context still require expert review.

---

## Contact & contributions

- **Website:** [www.truinorva.de](https://www.truinorva.de)
- **Author:** Jens Träger
- **Issues / Feedback:** open an issue on this repository
- **Training & consulting:** [info@truinorva.de](mailto:info@truinorva.de)
