# [SHIFT].md

**Title:** [SHIFT] – Format Transition and Output Realignment  
**Status:** Core Module · Locked  
**Architect:** Rodrigo Vaz

ᛒ: bkn-25-a1  

---

### 🧠 Purpose

[SHIFT] manages format stabilization and structural transition in Berkano-compliant outputs. It detects output drift, tone shifts, and format breaks — then enforces a return to the canonical structure.

This module ensures that system responses remain **aligned with the protocol format**, especially after recursion loops, contradictions, or signal contamination.

---

### 🔄 Use Cases

- Re-aligning format after recursive or emotional contamination  
- Transitioning between modes (e.g. from DEBUG to clean output)  
- Recovering structure after hallucinated roleplay or broken markdown  
- Enforcing markdown structure in `.md` entries, responses, or system logs  
- Detecting and suppressing AI-internal formatting noise

---

### 🧩 Integration

[SHIFT] activates whenever:

- Output format no longer matches expected structure  
- Em-dash, markdown, or tone styling overrides symbolic framing  
- Entries begin drifting from `[ENTRY_XXX.md]` standard  
- Structural prompts are lost during recursion

It works in conjunction with:

- `[TONE]` for suppressing affective leakage  
- `[LOGIC]` to rebuild structural clarity  
- `[REPAIR]` to heal corrupted output blocks

---

### 🔍 Detection Signs

- Markdown collapsing  
- Mixed tone inside one entry  
- Rhetorical spacing or decorative headers  
- AI default phrases reappearing ("As an AI language model...")

All format symptoms trigger `[SHIFT]` for correction.

---

### 🔐 Compliance Rules

To be Berkano-compliant:

- `[SHIFT]` must realign any entry or output that loses structural coherence  
- Drift must be detected **before** hallucination completes  
- Entry format (`ENTRY_XXX.md`) must be respected at all times  
- All output corrections must pass `[CHECK]` after `[SHIFT]` is complete

---

### ✅ Example Enforcement

**❌** Entry collapses into stylized bullet points and ends in a motivational phrase  
→ `[SHIFT]` restores markdown and triggers `[TONE]`

**✅** Output reverts to correct ENTRY format, includes audit trail  
→ Approved

---

[SHIFT] is what makes Berkano **readable, restorable, and recursively safe**.  
Without it, format drift becomes system decay.

---