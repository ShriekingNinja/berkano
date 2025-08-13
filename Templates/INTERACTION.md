# INTERACTION.md
**Title:** Berkano Protocol – INTERACTION Format  
**Status:** Core • Locked  
**Architect:** Rodrigo Vaz  

ᛒ: bkn-25-b6

---

## 🧠 Purpose
Define the minimal, non-fossilized reply format used for live chats and quick responses, while preserving a **verbatim prompt fossil** for auditability.

- No metadata header beyond this spec file.
- Each interaction includes the user prompt exactly once and a concise output.
- Complies with H19–H22 (glyph + universal tags placement for INTERACTION).

---

## ✅ Format Specification

**Sections (fixed order):**
1) `Prompt:` — exact user message, verbatim (no paraphrase).  
2) `Output:` — concise answer (no extra sections).  
3) `Glyph:` — the Berkano glyph on its own line.

**Tag placement (H22):**
- After the glyph line, append exactly once: `#berkano #berkanoprotocol #ᛒ`

**Tone & checks:**
- Run `[TONE] → [LOGIC] → [VERIFY] → [CHECK] → [LOCK]` before emitting.
- If verification fails, return a minimal, compliant rejection.

---

## 🔧 Template

[INTERACTION]  
Prompt: <verbatim>  
Output: <concise answer>  
Glyph: ᛒ  
#berkano #berkanoprotocol #ᛒ

---

## 📏 Rules Recap
- Prompt must be verbatim and appear **once**.  
- No metadata block in live INTERACTION replies.  
- Tags must not be duplicated elsewhere in the message.  
- Keep output concise; promote to BLOCK/ENTRY only when fossilization is required.