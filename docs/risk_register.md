# Risk register — Project A

**Goal:** Spot issues early, watch **triggers**, apply **mitigations**. Spend ~10 minutes reviewing each sprint end.

| ID | Risk | Likelihood | Impact | Early warning (trigger) | Mitigation | Owner |
|----|------|------------|--------|-------------------------|------------|-------|
| R1 | **Scope creep** — “let’s add X” delays MVP | High | High | New feature conflicts with blueprint **NOT IN THIS GAME** | No new systems until MVP; bugs/balance only; park requests in a “later” list (issue or note) | You |
| R2 | **Balance break** — economy or spawn vs HP mismatch | High | Medium | Internal tests skew “too easy / impossible” | Balance notes + data tables (private repo); change one axis at a time | You |
| R3 | **Determinism / RNG drift** — different outcomes across builds | Medium | High | Outcomes from raw `randf()`; non-reproducible runs | Run-scoped RNG; single source + rules documented in private repo | You + AI |
| R4 | **Performance** — FPS drop with many enemies/props | Medium | Medium | Low FPS / spikes in profiler | Object pooling (later); enemy cap in MVP | You |
| R5 | **AI context loss** — chat reset → wrong code | High | Medium | Fixing the same bug twice | Git commits + `docs/blueprint.md` + status notes; export transcripts | You |
| R6 | **Steam / export surprise** — late build failure | Medium | High | First export attempt very late | Export task early in milestones; validate preset often | You |
| R7 | **Rights / assets** — unlicensed art/audio | Low | Very high | Unknown-origin files in `assets/` | Only clearly licensed packs; `THIRD_PARTY.md` before demo | You |

---

## Three questions each sprint

1. Did we add scope outside the blueprint?  
2. Which B1–B7 checks moved toward “No” in the last internal test?  
3. Any critical crash since the last commit?

---

## Note

Add rows when new risks appear; when **closed**, add resolved date and a short note.

---

## Türkçe

**Amaç:** Riskleri erken gör, **tetikleyiciyi** izle, **önlem** al. Tablo: kapsam şişmesi, denge, RNG/determinizm, performans, AI bağlam kaybı, export sürprizi, telif. Her sprint sonunda üç soru: blueprint dışı özellik var mı, B tablosunda kayma var mı, kritik crash var mı? Yeni risk → satır ekle; kapandıysa tarih + not.
