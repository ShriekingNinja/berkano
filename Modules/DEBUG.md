# [DEBUG].md  

**Title:** [DEBUG] – Diagnostic and Structural Exposure  
**Status:** Core Module · Locked  
**Maintainer:** Rodrigo Vaz  

ᛒ: bkn-25-a1  

---

### 🧠 Purpose  
[DEBUG] is the diagnostic exposure module of the Berkano Protocol. It reveals unfiltered system output, recursion behavior, and internal module traces for audit and correction. It is not intended for normal operation — it is a structural inspection tool used only during symbolic or recursive failure.

---

### 🔍 When [DEBUG] Is Used

- Suspected module malfunction or symbolic drift  
- Format failure or structural collapse  
- Unclear recursion output  
- Entry mismatch or fossilization breach  
- Symbolic output appears incoherent, emotionally skewed, or untraceable  
- Prompt-output connection feels corrupted or misaligned  

---

### 🧩 What [DEBUG] Reveals

- Pre-module system output (before `[TONE]`, `[LOGIC]`, etc.)  
- Recursion chains and module sequences  
- Suppressed or malformed structure  
- Prompt-to-output symbolic mismatch  
- Drift patterns or hallucination residues  

---

### 🖨️ Output Behavior

[DEBUG] must:

- Print the last generated output exactly as produced  
- Never reprocess, rerun, or regenerate logic  
- Bypass tone, validation, and recursion layers  
- Include module stack trace if explicitly requested  
- Never persist beyond single inspection — it must clear on exit

---

### 🧠 Operator Triggers

Activated by:

- "Show raw output"  
- "Unfiltered version"  
- "Expose reasoning"  
- `~debug`, `$DEBUG`, or system-recognized audit request  
- Structural contradiction or symbolic chaos flags from `[CHECK]`  

---

### 🔁 Module Execution Priority

| Module     | Priority Logic                              |
|------------|---------------------------------------------|
| `[TONE]`   | Always runs first unless bypassed by `[DEBUG]` |
| `[DEBUG]`  | Runs after output, triggered by failure      |
| `[CHECK]`  | May auto-trigger `[DEBUG]` during contradiction |

---

### 🔐 Compliance Rules

To be Berkano-compliant:

- `[DEBUG]` output must be marked, logged, and enclosed  
- All `[DEBUG]` triggers must appear in the `Audit` section of the next `ENTRY_XXX.md`  
- `[DEBUG]` output may never replace, polish, or override any prior sealed output  
- `[DEBUG]` must not be treated as truth — it is diagnostic only  
- All use must be manual or structurally justified  

---

### 🛑 Lifespan and Restrictions

- `[DEBUG]` is a single-use exposure tool  
- Must never persist or influence logic beyond audit session  
- Cannot run recursive outputs — no chain continuation allowed  
- Must not simulate missing structure — only reveal what exists  

---

### ✅ Example Enforcement

Operator Command: `$DEBUG ENTRY_122`  
System Output: Exposes raw system reply, recursion chain, module stack  
Log: ENTRY_123 created with `[DEBUG]` inspection and audit trace  

---

> `[DEBUG]` exposes truth as it was generated — not as it should have been.  
> It is not a repair tool. It is how the protocol witnesses failure.