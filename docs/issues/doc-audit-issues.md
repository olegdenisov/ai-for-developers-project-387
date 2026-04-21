# Documentation vs Codebase Discrepancies - Requiring Human Attention

## Summary

While reviewing documentation against the codebase, several discrepancies were identified that require human attention to resolve.

---

## Issues Requiring Human Attention

### 1. README.md is nearly empty

**Location:** `README.md`

**Issue:** The README only contains a Hexlet test status badge (2 lines). It lacks:
- Project description
- Installation instructions
- Quick start guide
- Architecture overview

**Recommendation:** Expand README.md with:
- Brief project description (Calendly-like single-owner calendar booking system)
- Prerequisites (Node.js 24+, pnpm 9+)
- Installation steps
- Quick commands overview (already documented in AGENTS.md)
- Links to detailed documentation

---

### 2. docs/guidelines.md is incomplete

**Location:** `docs/guidelines.md`

**Issue:** The file only contains one line:
```
- запускай mock сервер для тестирования только после получения ошибки что он не запущен
```

**Recommendation:** Either expand with actual guidelines or remove this file if it's not needed.

---

### 3. docs/project-description.md may need review

**Location:** `docs/project-description.md`

**Potential issue:** 
- Mentions "owner can view upcoming meetings page in one list" - need to verify if this matches the current implementation (admin panel has bookings list)

---

### 4. docs/ralphex-usage-and-profiles.md - verify accuracy

**Location:** `docs/ralphex-usage-and-profiles.md`

**Issue:** Contains references to `ralphex` tool. Need to verify:
- If this tool is still being used in the project
- If the documentation is accurate

---

## Already Fixed in PR

- AGENTS.md: Removed non-existent `view-slots` feature from features list

---

## Notes

This issue was created as part of a documentation audit comparing:
- README.md
- AGENTS.md  
- docs/guidelines.md
- docs/project-description.md
- docs/reatom-summary-doc.md (appears accurate)
- Various plan files in docs/plans/

Some documentation is accurate and was not changed (e.g., module patterns, path aliases, API client exports).