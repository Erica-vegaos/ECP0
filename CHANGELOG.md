# Changelog — ECP0 Tone Governance Protocol  
_All entries are timestamped (UTC+8 · Asia/Taipei) for audit & licence traceability._

---

## [v1.1.1-O] — 2025-05-04  

### Added  
- **Bilingual README** — `README_Tone_Governance_DEF.en.md` & `.zh.md` published at repo root.  
- **CHANGELOG.md** now stored under `/docs/` with version tag export for CI.  
- **Glossary v1.0 CSV** auto-generated for Notion sync (`/docs/glossary.csv`).  

### Changed  
- Vocabulary Lock-in Map trimmed to *public subset*; internal terms removed.  
- CI workflow updated:  
  - `make_sha.py` now ignores `/docs/TO_BE_RELEASED/**` and glossary CSV.  
  - `check_glossary_conflict.py` enforces 300-term lock across commits.  
- README links adjusted to absolute paths for GitHub Pages rendering.  

### Security  
- Draft files require explicit `draft_only` front-matter; violation fails CI.  
- All newly exported PDF/SVG carry “ECP0 v1.1-O” watermark in footer.  

**Maintainer:** Eriga Enrich Inc. **Author:** Erica Wang 

---

## [v1.1-O] — 2025-04-25  

### Added  
- **Open-Core Edition** established  
  - Public clauses: TX01 (SafeMirror) · TX04 (Structural Observer)  
  - Sandbox Lite endpoints: TX02-Lite, TX05-Lite  
- **Initial README_Tone_Governance_DEF (draft)** with Semantic Protection Notice  
- **TAL-E Licence** upgraded to **v1.1-O** (effective date, token cap, UNCITRAL clause)  
- **Glossary v1.0** — 300 locked terms in `/docs/glossary.md`  
- **JSON templates** `/templates/TX_template.json` · `/templates/M_template.json`  
- **Draft isolation** folder `/docs/TO_BE_RELEASED/` (CI auto-skip)  

### Changed  
- Full TX02 – TX05 migrated to private repo; only Lite versions remain public  
- Repo split into `public/tx/` & `enterprise/tx/`; SHA auto-generation added  
- CI workflow: `check_draft_labels` & `make_sha.py` steps introduced  

### Security  
- Clause-level fingerprints saved to `/metadata/index.json`; README lists hashes  
- PDF/SVG exports embed “ECP0” watermark  

**Maintainer:** Eriga Enrich Inc. **Author:** Erica  

---

## [v1.0.0] — 2025-04-09  

### Added  
- Initial release of **ECP0 Tone Governance Protocol**  
- Published TX01 – TX05 core clauses  
- Issued **TAL-E Licence v1.0**  
- Scaffolded API-bound metadata & modular extensions  

**Maintainer:** Eriga Enrich Inc. **Author:** Erica  
