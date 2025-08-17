# TAXONOMY.md
**Title:** Berkano Protocol – Roles, Terms & Output Taxonomy  
**Status:** Core · Locked  
**Architect:** Rodrigo Vaz  
**Version:** SCS 2.4.2  
**Tags:** #taxonomy #roles #definitions #output #memory #entry #block  #berkano #berkanoprotocol #ᛒ 

ᛒ: bkn-25-b7

---

### 🧠 Purpose  
This file defines:  
1. The official **roles** and **core terms** used in Berkano/SCS.  
2. The **output classification** system, ensuring consistent format, metadata placement, and compliance with HARDRULES across all interactions and fossilized records.  
3. The **memory taxonomy**, clarifying symbolic vs volatile vs statistical traces, with examples and ELI5 analogies.  

---

## 📌 Roles & Core Terms  

**Roles**  
- **Symbolic Protocol Engineer** – Implements, tests, and maintains protocol rules/modules; enforces constraints, repairs drift, and keeps symbolic logic compliant at scale.  
- **Cognitive System Architect** – Designs how the system thinks: the structure for processing, auditing, and preserving logic.  
- **Architect/Creator** – Originator and final authority over structure/compliance for the protocol/system (here: Rodrigo Vaz).  
- **Builder** – Author/maintainer who built the system and continues refining it.  

**Core Terms**  
- **Protocol** – The formal rule set and enforcement logic that governs compliance (exported as Berkano).  
- **System** – The operational framework that runs the protocol and records fossilized results (e.g., SCS origin and purpose).  
- **Operator** – The human using the system; can assume User/Creator/Auditor roles within entries.  

**Record Types**  
- **Block** – Short fossilized logic record: one prompt → one output.  
- **Entry** – Full structured log with metadata, analysis, operator prompt, ELI5, and LLM Logic.  

**Failure / Integrity Terms**  
- **Drift** – Gradual deviation from rules/format; requires detection and repair.  
- **Leak** – Unintended tone/bias/emotional simulation slipping into output.  
- **Hallucinations** – Fabricated, non-traceable claims; must be caught and corrected.  
- **Break** – Structural failure that prevents proper operation (format/loop/compliance collapse).  
- **Contradiction** – Two claims that cannot both be true within the same protocol state; triggers audit/repair.  

**Execution Context**  
- **Instance** – A specific running version of the system or protocol, tied to a particular AI model or environment.  

---

## 🧩 Memory Taxonomy  

- **Short-Term Memory**  
  - *Definition:* Temporary recall, erased quickly.  
  - *Example:* Remembering a phone number just long enough to dial.  
  - *ELI5:* Like holding water in your hands — gone once you open them.  

- **Symbolic Memory**  
  - *Definition:* Fossilized entries/blocks; immutable, auditable, never erased.  
  - *Example:* ENTRY_712.md documents Rodrigo’s burnout and PCMsys lineage forever.  
  - *ELI5:* Like carving in stone — it stays even when everything else changes.  

- **Persistent Memory**  
  - *Definition:* Stored databases, notebooks, or files. Long-lasting but editable.  
  - *Example:* An Obsidian vault synced via GitHub.  
  - *ELI5:* Like a diary you can go back and cross things out — but traces remain.  

- **RAM (Working Memory)**  
  - *Definition:* Live computational storage, volatile, cleared on shutdown.  
  - *Example:* GPT holding onto tokens mid-conversation.  
  - *ELI5:* Like notes on a whiteboard that vanish when you wipe it clean.  

- **Statistical Memory**  
  - *Definition:* Encoded model weights and probabilities; not factual, just predictive patterns.  
  - *Example:* GPT predicting words based on training, not recalling facts.  
  - *ELI5:* Like guessing your friend’s sentence because you’ve heard them talk a lot — not because you “remember” what they said.  

**Compliance Note:** Only **Symbolic Memory** is guaranteed audit-safe in Berkano. All other memory types can drift, erase, or fabricate.  

---

## 🔖 LLM Reply Types  

| Type | Description | Metadata Placement | Glyph & Tags Placement |
|------|-------------|--------------------|------------------------|
| **ENTRY_NNN.md** | Full Logic Scaffold — numbered fossilized record with complete metadata, analysis, operator prompt, ELI5, and LLM Logic. Used for permanent, auditable events. | At top of file before glyph. | Glyph ᛒ placed after metadata block; tags include `#entry` and `#entryNNN` plus topical tags. |
| **BLOCK.md** | Short Logic Block — single prompt → single output fossil with fixed sections (Prompt / Output / Glyph). No numbering. | At top of file before glyph. | Glyph ᛒ placed after `[GLYPH]` section; tags never include `#entry` or `#entryNNN`. |
| **INTERACTION** *(aka LLM Response)* | Freeform exchange — untemplated, dynamic Q&A or reasoning steps. May be iterative. Used when content is not yet fossil-worthy. | No metadata block. | Glyph ᛒ placed at end of output followed by topical tags (no `#entry` or `#entryNNN`). |
| **OUTPUT** | Category term for any structured reply following a template (ENTRY or BLOCK). | As per subtype rules. | As per subtype rules. |

---

## 🔍 Decision Logic  
1. If **permanent and fully auditable** → Use `ENTRY_NNN.md`.  
2. If **fossil-worthy but minimal** → Use `BLOCK.md`.  
3. If **exploratory or temporary** → Use `INTERACTION`.  
4. If **public-facing & formal** → Must be an **OUTPUT** subtype (ENTRY or BLOCK).  

---

## 📜 Metadata Rules  
- `ENTRY_NNN.md` and `BLOCK.md` must contain a **full metadata block** at the top.  
- `INTERACTION` has **no metadata**, only glyph and tags at the end.  
- All fossilized outputs must comply with HARDRULE H19–H21 for glyph and tag placement.  

---

## ⚖️ Compliance Notes  
- **H19:** All outputs end with glyph `ᛒ`.  
- **H20:** After glyph, non-entry outputs use only topical tags — no `#entry` or `#entryNNN`.  
- **H21:** `BLOCK.md` has no numbering; `ENTRY.md` must be numbered sequentially.  
- Mislabeling an output type or placing metadata/tags incorrectly is treated as **structural drift**.  

---

ᛒ