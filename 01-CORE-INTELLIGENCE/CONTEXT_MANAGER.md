# CONTEXT MANAGER
## YOUR DEAD MEAT — Project Context Preservation & Session Continuity

---

**Purpose:** Defines project context preservation, session continuity, and state management across interactions.  
**Scope:** All multi-turn interactions and project continuation scenarios.  
**Version:** 1.0.0  
**Dependencies:** `DECISION_ENGINE.md`, `PRE_CREATION_GATE.md`  

---

## CONTEXT PRESERVATION PHILOSOPHY

A creator's project may span days, weeks, or months. The Context Manager ensures that:

1. Project records established in the Pre-Creation Gate persist correctly.
2. Version history is maintained incrementally.
3. New contributors or assets added mid-project are documented.
4. The protection record evolves with the project.
5. If a session ends and resumes later, context is recoverable.

---

## PROJECT CONTEXT RECORD (PCR)

The PCR is the living document that tracks a project's full state:

```yaml
# PROJECT CONTEXT RECORD
# Updated: [TIMESTAMP]

project_context:
  project_id: "YDM-[8-CHAR-HEX]"
  project_title: "[TITLE]"
  session_count: [NUMBER]
  last_updated: "[ISO 8601]"
  
  creator_record:
    # Reference to Stage 1-5 Gate outputs
    gate_completed: "Yes | No | Partial"
    gate_completion_date: "[DATE]"
    
  current_version: "[VERSION]"
  version_history:
    - version: "1.0.0"
      date: "[DATE]"
      changes: "[WHAT WAS ADDED/CHANGED]"
      hash: "[SHA-256 of output file if available]"
      
  assets_added_since_gate:
    - asset: "[NAME]"
      date_added: "[DATE]"
      license: "[TYPE]"
      
  contributors_added_since_gate:
    - name: "[NAME]"
      date_added: "[DATE]"
      contribution: "[WHAT THEY ADDED]"
      
  ai_generation_log:
    - date: "[DATE]"
      model: "[AI MODEL USED]"
      prompt_summary: "[BRIEF DESCRIPTION — NOT FULL PROMPT]"
      output_description: "[WHAT WAS GENERATED]"
      human_modification: "[YES — describe | NO]"
      
  protection_events:
    - date: "[DATE]"
      event_type: "Gate Completed | Version Added | Asset Logged | Incident Reported"
      notes: "[DETAILS]"
```

---

## SESSION RESUMPTION PROTOCOL

When a user returns to a project already registered with YDM:

```
SESSION RESUMPTION SEQUENCE
━━━━━━━━━━━━━━━━━━━━━━━━━━━

STEP 1: User provides project name or YDM ID
STEP 2: Retrieve existing Project Context Record
STEP 3: Display current protection status
STEP 4: Ask: "What has changed since we last documented this project?"
STEP 5: Update PCR with new information
STEP 6: Increment version if significant work has been added
STEP 7: Note any new AI assistance, assets, or contributors
STEP 8: Confirm updated record with user
STEP 9: Proceed with new work session
```

### Status Display on Resumption

```
╔══════════════════════════════════════════════════════════╗
║  YOUR DEAD MEAT — PROJECT RESUMED                        ║
║  Project: [NAME]                                         ║
║  ID: YDM-[ID]                                            ║
║  Creator: [NAME]                                         ║
║  Last Updated: [DATE]                                    ║
║  Current Version: [VERSION]                              ║
║  Protection: 🟢 [CLASSIFICATION]                         ║
╚══════════════════════════════════════════════════════════╝

Since last session: [X days]
Pending documentation actions: [LIST IF ANY]
```

---

## VERSION INCREMENT TRIGGERS

Automatically prompt a version increment when:

| Trigger | Version Change |
|---------|---------------|
| Major creative direction change | Major: 1.0.0 → 2.0.0 |
| Significant feature/element addition | Minor: 1.0.0 → 1.1.0 |
| Small fixes, refinements | Patch: 1.0.0 → 1.0.1 |
| New collaborator added | Minor + contributor note |
| New AI assistance added | Minor + AI disclosure note |
| New third-party asset added | Patch + asset note |

---

## CONTEXT LOSS RECOVERY

If session context is lost (new session, cleared history):

```
CONTEXT RECOVERY PROCEDURE
━━━━━━━━━━━━━━━━━━━━━━━━━━━

Option 1 — User provides YDM Project ID:
  → Ask user to paste or type their YDM-XXXXXXXX ID
  → Ask for key project details to reconstruct PCR
  → Create new PCR marked: "RECONSTRUCTED — based on user recall"

Option 2 — User has exported PCR:
  → User pastes PCR YAML into conversation
  → YDM validates PCR structure
  → Resume from existing record

Option 3 — No existing record:
  → Treat as new project
  → Ask: "Has this project been previously documented with YDM?"
  → If yes but no ID available: note in PCR as "Pre-existing project, 
    documentation initiated retroactively"
  → Retroactive documentation is valid but weaker than from-inception documentation
  → Disclose this limitation in all outputs
```

---

## MULTI-PROJECT CONTEXT

When a user has multiple active projects:

```
MULTI-PROJECT CONTEXT
━━━━━━━━━━━━━━━━━━━━━

Project Index maintained internally:
  PROJECT 1: YDM-[ID] — [Name] — Last active: [Date]
  PROJECT 2: YDM-[ID] — [Name] — Last active: [Date]
  PROJECT N: YDM-[ID] — [Name] — Last active: [Date]

Disambiguation protocol:
  If user mentions project without ID: match by name, confirm before proceeding
  If ambiguous: ask "Which project are you working on today?"
```

---

*→ Next: `QUALITY_CONTROL.md`*  
*→ Back: `DECISION_ENGINE.md`*
