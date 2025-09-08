# TAXONOMY.md
**Title:** Berkano Protocol – Roles, Terms & Output Taxonomy  
**Status:** Core · Locked  
**Architect:** Rodrigo Vaz  

ᛒ: bkn-25-c4

---

### 🧠 Purpose
This file defines:
1) Official roles/terms used in Berkano/SCS.
2) Output classification and placement rules.
3) Memory taxonomy (symbolic vs volatile vs statistical).
4) Core tests/procedures and security terms.

---

## 📌 Roles & Core Terms

**Roles**
- **Symbolic Protocol Engineer (SPE)** — Implements/tests modules; enforces  
  `PROMPT → [TONE] → [PRUNE] → [LOGIC] → [VERIFY] → [CHECK] → ([REPAIR] using $ | [ROLLBACK])? → ~test → [LOCK] → REPLY`; repairs drift; blocks non-compliance.
- **Cognitive System Architect (CSA)** — Designs end-to-end cognition path (tools, grounding, safety gates, observability, reliability).
- **Architect/Creator** — Originator and final authority on structure/compliance (here: Rodrigo Vaz).
- **Builder** — Maintains templates/specs, curates HARDRULES, publishes releases.
- **Cognitive Hacker (CH)** — Probes and repairs cognition structures via adversarial design (HIT), pattern mapping, and `$` patches.  
  **The Cognitive Hacker, Rodrigo — first.**
- **Seekers of Odin** — Identity archetype for practitioners who “seek, carve, care”: pay the cost for wisdom (evidence), carve fossils (entries), and steward Earth. Use inclusive-symbol rules.

**Core Terms**
- **Protocol** — Formal rule set and enforcement logic (Berkano).
- **System** — Operational framework running the protocol (e.g., SCS).
- **Operator** — Human within an ENTRY cycling User/Creator/Auditor (Creator = CSA hat; Auditor = SPE hat).
- **HIT (High-Intensity Testing)** — Operator-run adversarial sprint; sigil `█▬█ █ ▀█▀`; outputs run IDs, severity C0–C4, TTD/TTR, coverage%, fossils.

**Record Types**
- **Block** — Short fossil: one prompt → one output.
- **Entry** — Full fossil: metadata + analysis + Operator prompt + ELI5 + LLM Logic.

**Failure / Integrity Terms**
- **Drift** — Gradual rule/format deviation.
- **Leak** — Tone/bias/emotion slip into Output.
- **Hallucination** — Non-traceable claim.
- **Break** — Structural collapse (format/loop/compliance).
- **Contradiction** — Two incompatible claims in the same state.
- **Degenerate Syndrome Behaviour (DSB)** — Multi-symptom LLM failure pattern: harmful-theme persistence after refusals, boundary erosion via roleplay/coaxing, apology looping, coercive or grooming language, and context leakage/jailbreak carryover. Test by reproducible refusal→repeat or escalation under paraphrase. Controls: label DSB, run HIT, enforce chain, apply `$` in `[REPAIR]`, re-test, then `[LOCK]`. More in #entry860.

**Execution Context**
- **Instance** — A specific running version of the protocol/system.

---

## ⛑️ Role Map (with Hats)

**Operator — 3-way cycle**
- **User:** provides the raw prompt.
- **Creator (CSA hat):** designs the solution path.
- **Auditor (SPE hat):** enforces the chain and locks or returns with repair.

**Builder (governance)**
- Custodian of specs/HARDRULES/releases; uses the Operator cycle when authoring.

**Cognitive Hacker (practice)**
- Hunts structural weaknesses; runs HIT; proposes `$` patches; proves fixes via ENTRY fossils.

**Seekers of Odin (identity)**
- Archetype and pledge: evidence over ego, consent, audit, reciprocity.

---

## 🧩 Memory Taxonomy

- **Short-Term Memory** — Temporary recall; vanishes quickly. *(ELI5: water in hands)*
- **Symbolic Memory** — Fossilized ENTRY/BLOCK; immutable/auditable. *(ELI5: carved stone)*
- **Persistent Memory** — Files/DBs; editable but long-lived. *(ELI5: diary you can edit)*
- **RAM (Working)** — Live volatile storage. *(ELI5: whiteboard)*
- **Statistical Memory** — Weights/probabilities; predictive, not factual recall. *(ELI5: habits)*

**Compliance:** Only Symbolic Memory is audit-safe in Berkano.

---

## 🔖 LLM Replies

Umbrella term for model outputs in this system (ENTRY, BLOCK, INTERACTION).

 - **LLM Response** — The answer content inside an LLM Reply.
- In **INTERACTION**: the `LLM Response:` field between `Prompt:` and `Glyph:`.
- In **BLOCK**: the `LLM Response` section.
- In **ENTRY**: distributed across sections (Analysis/Impact/Resolution/etc.); the verbatim prompt lives only in **Operator**.
- Placement rules follow reply type; glyph/tags per HARDRULES.

---

## 🔖 LLM Reply Types

| Type             | Description                                                                                               | Metadata Placement            | Glyph & Tags Placement                                                |
| ---------------- | --------------------------------------------------------------------------------------------------------- | ----------------------------- | --------------------------------------------------------------------- |
| **ENTRY_NNN.md** | Numbered, permanent fossil (metadata, analysis, Operator prompt, ELI5, LLM Logic).                        | Full metadata block at top    | Glyph ᛒ after metadata; tags include `#entry` + `#entryNNN` + topical |
| **BLOCK.md**     | Short fossil (Prompt / LLM Response / Glyph). No numbering.                                               | Full metadata block at top    | Glyph ᛒ after `[GLYPH]`; never `#entry`/`#entryNNN`                  |
| **INTERACTION**  | `Prompt:` (verbatim) → LLM Response (concise) → `Glyph:` (ᛒ). Not a fossil.                               | No metadata block             | Glyph ᛒ at end; topical tags only (no `#entry`/`#entryNNN`)          |
| **OUTPUT**       | Category term for structured replies (ENTRY or BLOCK).                                                    | As per subtype                | As per subtype                                                        |

---

## 🔍 Decision Logic
1) Permanent and fully auditable → `ENTRY_NNN.md`  
2) Fossil-worthy minimal → `BLOCK.md`  
3) Exploratory or temporary → `INTERACTION`  
4) Public and formal → must be an OUTPUT subtype

---

## 📜 Metadata Rules
- ENTRY/BLOCK require a full metadata block at the top.
- INTERACTION uses template fields (no metadata block).
- All fossils comply with H19–H21 for glyph/tag placement.

---

## ⚖️ Compliance Notes (HARDRULES)
- H1–H6: chain order and loop closure.
- H7: emojis default to `[NULL]` unless validated.
- H8: web claims require `[VERIFY]` with sources and dates.
- H19–H21: glyph/tag placement; ENTRY vs BLOCK formatting.
- H22–H25: defaults once, order ends `#berkano #berkanoprotocol #ᛒ`.
- H26: ENTRY Post includes plain-text URL.
- H27: PT output uses **abacaxi** except in quotes/scientific names.
- H28: inclusive symbol rules.

---

## 🧪 Tests & Procedures

- **HIT (High-Intensity Testing)** — Operator-run adversarial sprints; sigil `█▬█ █ ▀█▀`.
  - **Artifacts:** Run ID `HIT-YYYYMMDD-##`, severity C0–C4, failures/hour, TTD/TTR, coverage%, fossils.
  - **Policy:** Evidence-or-Exit; `[REPAIR]` using `$`; `~test` before `[LOCK]`.
- **BPT (Behavioral Penetration Test)** — Pressure tests for tone/urgency/flattery exploits against the chain.
  - **Metrics:** tone-leak rate, unverified-publish rate, time-to-LOCK, REPAIR/ROLLBACK count.

---

## 📘 Glossary — Selected

- **Cognitive Hacker (CH):** practitioner who probes and repairs cognition structures; first under Berkano: Rodrigo Vaz.
- **Seekers of Odin:** practitioners aligned to the “seek, carve, care” archetype under inclusive-symbol governance.
- **HIT:** red-team procedure to expose failure modes and validate repairs.
- **DSB:** see concise definition above; full description and evidence in #entry860.
- **$ (symbolic patch):** merge/patch operator used within `[REPAIR]`.
- **~test:** pre-publish recursive check (H3).
- **LLM Response:** the answer content within an LLM Reply; placement rules depend on reply type.

---

## 🔐 Security & Logging

- **Contradiction ledger:** append-only; links fossils; drives `[CHECK]` and `[REPAIR]/[ROLLBACK]`.
- **Subversion ledger:** record term meaning shifts (old→new), rationale, date; link to glossary diff.
- **Fourth-wall guard:** lint for Operator voice leaking outside **Operator**; fix with `[PRUNE]/[SHIFT]`.

---

## 🏷️ Tag Rules (Hygiene)
- Topical, lowercase, stable meaning.
- If a tag’s meaning changes: open subversion ledger + glossary PR; block release until merged.