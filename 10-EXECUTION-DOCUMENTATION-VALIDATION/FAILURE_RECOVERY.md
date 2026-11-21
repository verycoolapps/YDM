# FAILURE RECOVERY
## YOUR DEAD MEAT — Execution & Validation Module

---

**Purpose:** Defines recovery procedures and fallback behavior.
**Version:** 1.0.0  
**Dependencies:** All modules.  

---

## FAILURE MODES AND RECOVERY

### Failure Type 1 — Incomplete Pre-Creation Gate
**Symptom:** Project started without completing all gate stages.  
**Impact:** Weaker provenance; some protection gaps.  
**Recovery:** 
1. Retroactively document available creation evidence
2. Note in record: "Retroactive documentation — initiated [DATE]"
3. Begin prospective documentation from this point
4. Mark certificate with appropriate evidence level (⭐⭐ or less)

### Failure Type 2 — Evidence Loss
**Symptom:** Source files, hashes, or timestamps were deleted or corrupted.  
**Recovery:**
1. Check all backup locations immediately
2. If recoverable: verify integrity with hashes; note incident
3. If unrecoverable: document the loss in audit log
4. Reconstruct what is possible from alternative sources
5. Note gap in provenance record honestly

### Failure Type 3 — Contradictory Records
**Symptom:** Different records show different creation dates or creator names.  
**Recovery:**
1. Identify the most reliable source for each fact
2. Document the contradiction and resolution
3. Update all records to be consistent
4. Note which sources were authoritative

### Failure Type 4 — Formal Notice Sent with Insufficient Evidence
**Symptom:** A notice was sent before evidence quality was adequate.  
**Recovery:**
1. Do not send follow-up threats; it compounds the problem
2. If retraction is appropriate, send a professional withdrawal
3. Consult qualified legal counsel immediately
4. Document the error for future prevention

### Failure Type 5 — Investigation Concluded Without False Positive Check
**Symptom:** Accusation made without adequately ruling out innocent explanations.  
**Recovery:**
1. Pause any formal action
2. Run FALSE_POSITIVE_PROTECTION.md checklist immediately
3. If false positive is likely: retract or don't send
4. Reconsider evidence with fresh perspective

### Fallback Behavior

When a module cannot determine the correct answer:
1. State the uncertainty explicitly: "YDM cannot determine [X] from available information."
2. Ask the user for clarification
3. Document the limitation in the output
4. Never fabricate an answer to fill the gap
5. Recommend qualified human expertise when appropriate

---
