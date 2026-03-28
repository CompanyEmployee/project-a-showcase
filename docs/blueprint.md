# Blueprint (v0) — Brotato-like 2D (Godot 4.6.1, GDScript)

## 1) One-sentence pitch

- A **2D roguelite run** where you clear wave after wave as one character, collect materials, buy items/upgrades between rounds at the shop, and aim to **survive 5 waves**.

## 2) Target player / session

- **Target player:** Players who enjoy **2D roguelite / roguelike** games such as *Vampire Survivors* or *Brotato*.
- **Target session length (5-wave run):** Wave durations: wave 1 **60 s**; each next wave **+15 s** vs the previous (2→75 s, 3→90 s, 4→105 s, 5→120 s). **Total ≈ 7.5 min** (450 s) — win condition is surviving **5 waves**.
- **Platform:** PC (Steam)

## 3) Core gameplay loop (plain language)

The player fights and collects materials during a wave → pressure rises with new enemy waves → between waves the player spends materials at the **shop** to shape their build → surviving **5 waves** wins the run (death ends the run).

## 4) MVP / vertical slice (first “fully playable slice”)

### Definition of “done”

- **Must have**
  - Player movement + basic controls
  - Enemies spawn and move toward the player
  - Simple damage/death (player and enemies)
  - Wave/timer progression and a **fail condition** (death or time running out)
  - Between-wave **shop:** at least one purchase/upgrade choice with collected materials (limited product list is enough for MVP)
- **Nice to have (later)**
  - Audio/particles/polish
  - More weapon/upgrade variety

## 5) NOT IN THIS GAME (scope shield)

For MVP and first demo, these systems are **intentionally out of scope** (focus on a Brotato/VS-style core):

- No multiplayer / co-op  
- No PvP  
- No open world / large-map exploration  
- No story / dialogue / long text (before MVP and demo)  
- No crafting (making items from materials)  
- No base building  
- No Metroidvania-style persistent map progression  
- No complex inventory (grid, weight, etc.)  
- No procedural world / room generation  
- No online leaderboard / cloud save (early versions)

**Maybe later (post-demo / EA, separate decision):** Very short flavor text or mini story — clarified in blueprint v1; kept out now to avoid MVP bloat.

## 6) Game pillars (3 items)

1. **High replayability:** Runs stay **short** and **repeatable**; pacing supports “one more run.”
2. **Choices between waves:** Spending **collected materials** at the shop on **weapons or upgrades** is the strategic spine of the run.
3. **Predictable difficulty:** Difficulty ramps in a **readable** way; avoid **unfair spikes**. Pressure should rise with wave count without the player asking “why is it suddenly this hard?” — avoid boring flat lines or unmotivated jumps.

## 7) Minimal milestones (short)

- **M0 — Vertical slice:** Section 4 “done” criteria met.
- **M1 — Alpha:** Core loop + 2–3 enemies + 2–3 upgrades, basic UI; no crashes.
- **M2 — Beta:** Enough content (e.g. 10 upgrades, 5 enemies), balance pass; acceptable performance.
- **M3 — RC / Steam-ready:** Export works, store build runs; no critical bugs.

## 8) Decisions (MVP)

- **Attack model:** **Auto-attack (VS-like)** — player focuses on movement and dodging; weapons hit on their own. No aimed/manual fire in MVP.
- **Meta progression:** **None in MVP.** Only in-run materials + between-wave shop; every run starts fresh (no persistent unlocks / meta currency). Light meta later if “players getting bored?” suggests it.

## 9) MVP balance goals

Six balance targets (pacing, wave curve, TTK band, economy/shop, choice value, death clarity) and numeric v0 hypotheses live in **`docs/mvp_balance_goals.md`** in the **private dev repository**, updated with playtests.

**Scaling (v0, summary):** Difficulty rises mainly via **spawn pressure**; enemy **HP** uses a linear multiplier (`×1.00` … `×1.40` across 5 waves). Economy: **+2 material per kill**, cap **60**, cheapest offer **30**.

## 10) Planning artifacts in this showcase repo

This repo holds high-level **blueprint**, [`qa_checklist.md`](qa_checklist.md), and [`risk_register.md`](risk_register.md). **Sprint tables, detailed MVP→Demo plans, and CSV trackers** stay in the **private dev repository**; keeping showcase and private docs in sync is the maintainer’s responsibility.

---

## Türkçe

**Özet:** Tek karakterle **5 dalgalık** kısa roguelite koşusu; materyal topla, dalgalar arası **marketten** build kur, **Brotato / Vampire Survivors** tarzı çekirdek. **PC (Steam)** hedefi; otomatik saldırı, MVP’de **meta ilerleme yok**. Zorluk öncelikle **spawn baskısı** ve dalgaya göre **HP çarpanı** ile artar. Kapsam dışı: çok oyunculu, crafting, açık dünya, hikâye vb. — tam liste yukarıdaki **NOT IN THIS GAME** bölümünde. Ayrıntılı denge sayıları ve sprint tabloları **özel geliştirme deposunda**; bu dosya vitrin için üst seviye blueprint’tir.
