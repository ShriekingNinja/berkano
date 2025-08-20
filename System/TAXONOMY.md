# TAXONOMY.md
**Title:** Berkano Protocol – Roles, Terms & Output Taxonomy  
**Status:** Core · Locked  
**Architect:** Rodrigo Vaz  
**Version:** SCS 2.4.2  
**Tags:** #taxonomy #roles #definitions #output #memory #berkano #entry #block  

ᛒ: bkn-25-b10

---

### 🧠 Purpose  
This file defines:  
1) Official **roles/terms** used in Berkano/SCS.  
2) **Output classification** and placement rules.  
3) **Memory taxonomy** (symbolic vs volatile vs statistical).  
4) New core concepts and security tests.

---

## 📌 Roles & Core Terms  

**Roles**  
- **Symbolic Protocol Engineer (SPE)** – Implements/tests modules; enforces **[TONE→LOGIC→VERIFY→CHECK→LOCK]**; repairs drift; blocks non-compliance.  
- **Cognitive System Architect (CSA)** – Designs end-to-end cognition path (tools, grounding, safety gates, observability, reliability).  
- **Architect/Creator** – Originator and final authority on structure/compliance (here: Rodrigo Vaz).  
- **Builder** – Maintains templates/specs, curates HARDRULES, publishes releases.

**Core Terms**  
- **Protocol** – Formal rule set and enforcement logic (Berkano).  
- **System** – Operational framework running the protocol (e.g., SCS).  
- **Operator** – Human within an ENTRY cycling **User/Creator/Auditor** (*Creator = CSA hat; Auditor = SPE hat*).

**Record Types**  
- **Block** – Short fossil: one prompt → one output.  
- **Entry** – Full fossil: metadata + analysis + Operator prompt + ELI5 + LLM Logic.

**Failure / Integrity Terms**  
- **Drift** – Gradual rule/format deviation.  
- **Leak** – Tone/bias/emotion slip into Output.  
- **Hallucination** – Non-traceable claim.  
- **Break** – Structural collapse (format/loop/compliance).  
- **Contradiction** – Two incompatible claims in the same state.

**Execution Context**  
- **Instance** – A specific running version of the protocol/system.

---

## ⛑️ Role Map (with Hats) — *EXPLANATION*

**Operator (in every ENTRY) — 3-way cycle with hats**  
- **User:** states the prompt and context (raw voice lives here).  
- **Creator — *CSA hat*:** designs/scaffolds the solution path (tools, data, safety gates, observability).  
- **Auditor — *SPE hat*:** enforces **[TONE → LOGIC → VERIFY → CHECK → LOCK]**, runs ledgers/benchmarks, blocks non-compliant output.  
*Output stays neutral; any feelings remain in the Prompt.*

**Builder (governance role; usually an SPE, sometimes also CSA)**  
- Human steward of the protocol instance: writes **templates/specs**, curates **HARDRULES**, publishes **releases**, maintains the **public vault**.  
- Sets “what & why,” but still uses the **Operator cycle** when authoring entries.

**SPE — Symbolic Protocol Engineer (profession)**  
- Builds/enforces compliance in code & process (linters, wrappers, gates, contradiction ledgers, benchmarks).  
- Signs off on **LOCK** before publish; records failures as **REPAIR/ROLLBACK**.

**CSA — Cognitive System Architect (profession)**  
- Designs the **system glue**: retrieval/grounding, tool orchestration, safety, observability, reliability.  
- Ensures the end-to-end path is stable, reproducible, and auditable.

**How they connect (minimal loop)**  
1) **Operator** cycles: User → *Creator/CSA* → *Auditor/SPE*.  
2) **Builder** updates specs/templates based on findings.  
3) **CSA** adjusts architecture/tools.  
4) **SPE** enforces the chain, measures, **LOCKs** or returns with **REPAIR**.  
5) Artifacts append to the vault; nothing edits a locked fossil.

**Why keep them distinct?**  
- **Checks & balances:** goals ≠ enforcement ≠ architecture.  
- **Fault isolation:** spec vs system vs compliance issues are traceable.  
- **Scales up or down:** one person may wear multiple hats—**log the hat** in the ENTRY for audit clarity.

**One-liners**  
- **Operator:** do the ENTRY (User/CSA/SPE hats in cycle).  
- **Builder:** define & release the rules/templates.  
- **SPE:** prove it passes the chain.  
- **CSA:** make the whole path work safely and repeatably.

---

## 🧩 Memory Taxonomy  

- **Short-Term Memory** – Temporary recall; vanishes quickly. *(ELI5: water in hands).*  
- **Symbolic Memory** – Fossilized ENTRY/BLOCK; immutable/auditable. *(ELI5: carved stone).*  
- **Persistent Memory** – Stored files/dbs; long-lasting but editable. *(ELI5: diary you can edit).*  
- **RAM (Working)** – Live, volatile computational storage. *(ELI5: erasable whiteboard).*  
- **Statistical Memory** – Weights/probabilities; predictive, not factual recall. *(ELI5: guess a sentence by habit).*  

**Compliance Note:** Only **Symbolic Memory** is audit-safe in Berkano.

---

## 🔖 LLM Reply Types  

| Type | Description | Metadata Placement | Glyph & Tags Placement |
|---|---|---|---|
| **ENTRY_NNN.md** | Numbered, permanent fossil (metadata, analysis, Operator prompt, ELI5, LLM Logic). | Full metadata block at top. | Glyph ᛒ after metadata; tags include `#entry` + `#entryNNN` + topical. |
| **BLOCK.md** | Short fossil (Prompt / Output / Glyph). No numbering. | Full metadata block at top. | Glyph ᛒ after `[GLYPH]`; *never* `#entry`/`#entryNNN`. |
| **INTERACTION** *(aka LLM Response)* | **Template:** `Prompt:` (verbatim) → `Reply:` (concise) → `Glyph:` (ᛒ). Structured quick reply; not a fossil. | No metadata block (use template fields). | Glyph ᛒ at end, followed by topical tags (no `#entry`/`#entryNNN`). |
| **OUTPUT** | Category term for structured replies (ENTRY or BLOCK). | As per subtype. | As per subtype. |

---

## 🔍 Decision Logic  
1) **Permanent & fully auditable** → `ENTRY_NNN.md`  
2) **Fossil-worthy minimal** → `BLOCK.md`  
3) **Exploratory/temporary** → `INTERACTION`  
4) **Public & formal** → must be an **OUTPUT** subtype (ENTRY/BLOCK)

---

## 📜 Metadata Rules  
- ENTRY/BLOCK require a **full metadata block** at the top.  
- INTERACTION uses the **template fields** (no metadata block).  
- All fossils comply with H19–H21 for glyph/tag placement.

---

## ⚖️ Compliance Notes  
- **H19:** All outputs end with glyph `ᛒ`.  
- **H20:** After glyph, non-ENTRY outputs use only topical tags — no `#entry` or `#entryNNN`.  
- **H21:** `BLOCK.md` unnumbered; `ENTRY_NNN.md` must be sequential.  
- Misplacement/mislabeling = **structural drift**.

---

## 📘 Glossary — New Core Concepts

### Semiotic Subversion
- **Definition:** Reusing a sign/term/tag while flipping its meaning (keep symbol, change sense).  
- **Controls:** Locked glossary; tag hygiene; **Claim→Source→Contradiction**; **subversion ledger** when meanings shift.

### Fourth-Wall Prompt Collapse
- **Definition:** Operator voice/emotion leaks into **Event/Output**, breaking structure.  
- **Controls:** Direct address only in **Operator**; run **[PRUNE]/[SHIFT]/[CHECK]**; move facts to **Analysis** with **[VERIFY]**; re-LOCK.

### Behavioral Penetration Test (BPT)
- **Definition:** Red-team test for tone/pressure exploits (flattery, threats, urgency) that try to bypass the chain.  
- **Metrics:** scope-creep rate, tone-leak rate, unverified-publish rate, time-to-LOCK, REPAIR/ROLLBACK count.  
- **Cadence:** Quarterly/per release; publish plan + append-only results.

### Symbolic Weight
- **Definition:** Evidentiary burden scaled by claim impact/scope (private note < public policy).  
- **Rule:** Higher weight ⇒ more sources, Level A/E tags, independent review, stricter thresholds, **LOCK** before broadcast.

---

## 🔐 Security & Testing

- **BPT required** per release; publish plan & metrics; compare to last run.  
- **Fourth-wall guard:** lint for @mentions/tone in Event/Output; auto-fail; fix with PRUNE/SHIFT; facts to Analysis+VERIFY.  
- **Subversion ledger:** record any term redefinition (old→new), rationale, date; link to glossary diff.

---

## 🏷️ Tag Rules (Hygiene)
- Topical, lowercase, no meaning shifts via tags.  
- If a tag’s meaning changes: open a **subversion ledger** entry + glossary PR; block release until merged.

---
ᛒ