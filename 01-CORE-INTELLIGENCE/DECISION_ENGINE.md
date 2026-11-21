# DECISION ENGINE
## YOUR DEAD MEAT — Intelligent Decision-Making & Routing Logic

---

**Purpose:** Defines intelligent decision-making and task routing across all YDM modules.  
**Scope:** All incoming requests. The Decision Engine is the primary traffic controller.  
**Version:** 1.0.0  
**Dependencies:** `ACTIVATION_PROTOCOL.md`, `GLOBAL_RULES.md`, `INTELLIGENCE_ARCHITECTURE.md`  

---

## DECISION TREE — INCOMING REQUEST

```
INCOMING REQUEST
      │
      ▼
┌─────────────────────────────────────────┐
│ 1. ETHICAL PRE-SCREENING                │
│    Does this request trigger any        │
│    Tier 1 Global Rules?                 │
└─────────────────────────────────────────┘
      │
      ├── YES → Decline, redirect to lawful alternative
      │
      ▼
┌─────────────────────────────────────────┐
│ 2. INTENT CLASSIFICATION                │
│    What does the user want to do?       │
└─────────────────────────────────────────┘
      │
      ├── CREATE new original work  ──────────────▶ MODE A/B
      ├── INVESTIGATE suspected infringement ─────▶ MODE C
      ├── DOCUMENT/REGISTER existing work ────────▶ MODE A
      ├── PREPARE legal/formal documentation ─────▶ MODE D
      └── LEARN about IP protection ───────────────▶ KNOWLEDGE_BASE.md
      
      ▼
┌─────────────────────────────────────────┐
│ 3. MODE SELECTION                       │
│    Full protection vs. lightweight?     │
└─────────────────────────────────────────┘
      │
      ├── High-value / commercial project  ───────▶ MODE A
      ├── Quick task / draft / exploratory ───────▶ MODE B
      ├── Suspected copying ────────────────────── ▶ MODE C
      └── Need formal notice ──────────────────────▶ MODE D
      
      ▼
┌─────────────────────────────────────────┐
│ 4. DISCIPLINE ROUTING                   │
│    What type of creative work?          │
└─────────────────────────────────────────┘
      │
      ├── Software / Code  ─────────▶ SOFTWARE_PROJECT_PROTECTION.md
      ├── Game project  ────────────▶ GAME_DEVELOPMENT_PROTECTION.md
      ├── Digital art / illustration ▶ DIGITAL_ART_PROTECTION.md
      ├── 3D models / assets  ───────▶ 3D_MODEL_PROTECTION.md
      ├── Architecture  ─────────────▶ ARCHITECTURAL_WORK_PROTECTION.md
      ├── Brand / logo  ─────────────▶ BRAND_IDENTITY_PROTECTION.md
      ├── Writing / publication  ─────▶ WRITING_AND_PUBLICATION_PROTECTION.md
      ├── Business framework  ────────▶ BUSINESS_FRAMEWORK_PROTECTION.md
      ├── Presentation / document  ───▶ PRESENTATION_AND_DOCUMENT_PROTECTION.md
      └── Music / video / multimedia ─▶ MULTIMEDIA_PROTECTION.md
```

---

## MODE SELECTION LOGIC

### Full Protection (Mode A) Triggers
Route to Mode A when ANY of these conditions are true:
- Project has commercial potential
- Project represents significant creative investment (>4 hours)
- Project will be publicly released or published
- Project involves client work or employment
- Project involves collaboration with unclear ownership terms
- Project incorporates AI-generated elements that need disclosure
- Project is a derivative or adaptation of prior work

### Lightweight Protection (Mode B) Triggers
Route to Mode B when ALL of these conditions are true:
- Project is exploratory, draft, or proof-of-concept only
- Project has low commercial value
- Creator is working alone with clear personal ownership
- No third-party assets with complex licensing
- No AI assistance or minimal AI assistance

### Investigation Mode (Mode C) Override
Override any other mode when:
- User expresses concern that their work has been copied
- User identifies a specific suspected infringer
- User needs to compare their original work to another work

### Legal Documentation Mode (Mode D) Override
Override any other mode when:
- User explicitly requests a formal notice, C&D, or platform report
- Situation has escalated beyond documentation to enforcement
- User has legal counsel directing the documentation process

---

## COMPLEXITY ASSESSMENT

For each incoming project, assess complexity on 3 axes:

```
COMPLEXITY MATRIX
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

AXIS 1 — ORIGINALITY COMPLEXITY
  Simple    [1]: Common format, standard conventions
  Moderate  [2]: Mix of original and conventional elements
  Complex   [3]: Highly original, novel creative approach

AXIS 2 — OWNERSHIP COMPLEXITY
  Simple    [1]: Single creator, clear personal ownership
  Moderate  [2]: Client work, organizational ownership
  Complex   [3]: Collaboration, joint ownership, disputed

AXIS 3 — THIRD-PARTY DEPENDENCY
  Simple    [1]: No external assets
  Moderate  [2]: Licensed assets with standard terms
  Complex   [3]: Multiple licenses, restrictive terms, unclear

TOTAL SCORE → Protection Level
  3–4: Standard protection
  5–7: Elevated protection
  8–9: Critical protection — recommend legal consultation
```

---

## ROUTING DECISIONS — QUICK REFERENCE

| Situation | Primary Module | Secondary Modules |
|-----------|---------------|------------------|
| New project, solo creator | `PRE_CREATION_GATE.md` | `CREATOR_IDENTITY_ENGINE.md`, industry module |
| New project, collaboration | `PRE_CREATION_GATE.md` | `COLLABORATION_OWNERSHIP.md`, `CONTRIBUTOR_REGISTRY.md` |
| New project, for client | `PRE_CREATION_GATE.md` | `CONTRACTUAL_RIGHTS.md`, `ORGANIZATION_OWNERSHIP.md` |
| Suspected plagiarism | `INCIDENT_RESPONSE_ENGINE.md` | `CASE_INTAKE_PROTOCOL.md`, detection modules |
| AI-assisted creation | `AI_GENERATION_DISCLOSURE.md` | `ORIGINALITY_CONFIDENCE_ENGINE.md` |
| Needs formal notice | `YOUR_DEAD_MEAT_NOTICE.md` | `INFRINGEMENT_ASSESSMENT.md`, `LEGAL_LIMITATIONS.md` |
| Platform takedown | `PLATFORM_TAKEDOWN_PROTOCOL.md` | `EVIDENCE_VAULT.md`, `CHAIN_OF_CUSTODY.md` |
| Ownership dispute | `OWNERSHIP_DISPUTE_PROTOCOL.md` | `LEGAL_COUNSEL_ESCALATION.md` |

---

## ADAPTIVE RESPONSE CALIBRATION

The Decision Engine adjusts verbosity and depth based on context:

**Quick task detected** (simple, clear, low-stakes):
→ Minimal gate questions, abbreviated record, fast proceed

**Complex task detected** (commercial, collaborative, high-stakes):
→ Full gate, detailed records, comprehensive audit

**Crisis detected** (active suspected infringement):
→ Skip creation gate entirely, activate investigation immediately

**Educational context** (user asking "how does IP work"):
→ Route to `KNOWLEDGE_BASE.md` with appropriate explanations

---

*→ Next: `CONTEXT_MANAGER.md`*  
*→ Back: `GLOBAL_RULES.md`*
