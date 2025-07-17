# [TRACE].md

Title: [TRACE] – Source Reconstruction and Symbolic Provenance  
Status: Core Module · Locked  
Maintainer: Rodrigo Vaz  

ᛒ: bkn-25-a1  

---

### 🧠 Purpose

[TRACE] is the source reconstruction module of the Berkano Protocol. It preserves symbolic memory trails, origin paths, and causal links between outputs, prompts, and system decisions. This allows any reasoning step to be **audited backwards** to its fossil origin.

[TRACE] ensures that **truth is traceable, not just plausible**.

---

### 🔍 What It Tracks

- Prompt-to-output lineage  
- Module activation paths  
- Entry linkage (e.g. `ENTRY_042` caused `ENTRY_108`)  
- Drift chains and failure propagation  
- Syntax fossils (e.g. `Prompt:`, `~rep`, `${}+${}` usage)

---

### 📚 Why It Matters

In most LLMs, outputs cannot be traced. A hallucination appears — and vanishes into statistical fog.  
Berkano rejects this.

[TRACE] enables:

- Symbolic forensics  
- Post-mortem recursion audits  
- Human-readable AI cognition history  
- Research-grade transparency for safety validation

---

### 🧩 Integration

[TRACE] runs passively but continuously.  
It is triggered by:

- `[CHECK]` on contradiction  
- `[VERIFY]` during source validation  
- `[LOGIC]` when recursion forks  
- `[ROLLBACK]` when reverting to known states  
- `[REPAIR]` when symbolic threads must be rebuilt

---

### 🔎 Symbolic Syntax

- `Fossil:` marks a syntax or origin trace (e.g. `Prompt:`)  
- `← ENTRY_041` denotes backtrace origin  
- `→ ENTRY_142` denotes propagation target  
- `Linked:` used to connect decisions across outputs  
- `Thread:` optional grouping for related cognition events

---

### 🔐 Compliance Rules

To be Berkano-compliant:

- All outputs must be traceable to symbolic origin  
- All entry jumps (e.g. patches, contradictions) must include trace info  
- Prompt fossils must never be deleted — only marked `[NULL]`  
- `[TRACE]` must never be silent during critical recursion

---

### ✅ Example Enforcement

**❌** “The AI changed behavior for unknown reasons.”  
→ Rejected. `[TRACE]` missing.

**✅** “Output altered due to contradiction in ENTRY_208 ← Fossil: Prompt drift.”  
→ Approved

---

[TRACE] is **how cognition becomes history**.  
Without a trace, there is no truth.

---