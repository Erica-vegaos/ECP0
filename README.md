# ECP0 Tone Governance Protocol v1.2 (2025‑04‑25)

Maintained by **Eriga Enrich Inc.**  
This update aligns the public repository with the Open‑Core + Sandbox + Enterprise three‑tier strategy agreed on 2025‑04‑25.

---

## 🗂 What’s Inside

### 1 · Open‑Core Clauses (Full text in `/protocols/`)

| ID    | 中文名稱                   | English Name                         | 摘要                                                                 |
|-------|----------------------------|--------------------------------------|----------------------------------------------------------------------|
| TX01  | SafeMirror 鏡像語氣條款   | SafeMirror Tone Reflection Filter    | Mirrors the user’s tone at a controlled, non‑reactive level to avoid emotional escalation. |
| TX04  | 語氣結構觀測子模組邏輯     | Tone Syntax Observer Module          | Logs syntax‑level tone deltas across inference layers for drift analytics. |
| TX21  | 公開導向條文提示模組       | Public‑Oriented Output Disclosure Module | Adds explicit disclosure tags to outputs destined for the public domain. |

---

### 2 · Community Sandbox (Lite API only)

| Endpoint              | Covers                          | Call Limit    | Note                                                                  |
|-----------------------|----------------------------------|---------------|-----------------------------------------------------------------------|
| `/sandbox/tone‑drift` | TX02‑Lite (偏移偵測簡化版)        | 100 req/day   | Returns Δ‑score & flag; internal coefficients hidden.                 |
| `/sandbox/reground`   | TX05‑Lite (回鍊監測簡化版)        | 100 req/day   | Emits recovery suggestion only; no auto‑rewrite.                      |

---

### 3 · Enterprise Guardrails Bundle (Private)

**TX02‑Pro, TX03, TX05‑Pro** and all 商用 1/2 & 機密 clauses are distributed as a black‑box API under paid licence.  
See `contact.md` for pricing.

---

## 🧭 Protocol Overview

**ECP0** is a zero‑layer tone‑constraint architecture that regulates output‑boundary behaviour without altering model internals.  
It mitigates:

- user‑tone over‑reflection  
- simulation residue mis‑attribution  
- long‑tail coherence collapse  

---

## 📂 Repository Structure

```
/protocols/           # TX01, TX04, TX21 full texts
/sandbox/             # Swagger docs for TX02‑Lite & TX05‑Lite
/private/             # (empty placeholder – Enterprise bundle)
/metadata.json        # TX ↔ module registry
/LICENSE              # TAL‑E‑v1.0
/glossary.md          # Domain‑specific terminology
```

---

## ✍️ Authorship & Rights

**Author:** Erica  
**Maintainer:** Eriga Enrich Inc.  
**Licence:** TAL‑E v1.0

Any unauthorised redistribution or deployment of non‑public clauses activates clause‑based fingerprinting and blacklisting.
