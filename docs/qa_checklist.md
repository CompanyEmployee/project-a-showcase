# QA checklist — MVP and Demo

Use this form **solo or with a tester**. Mark each row **Yes / No / Partial**; add short notes in the **Notes** column.

**Build info (every session):**

- Date: 2026-03-28 (MVP-22 freeze + tag `mvp-0.1`)
- Build / commit: `git rev-parse --short HEAD` — verify locally
- Platform: Windows (Steam target)
- Input: keyboard (WASD) + mouse (menu/shop)

*MVP-01:* `scenes/`, `scripts/`, `resources/`, `assets/` layout; project opens (A1).  
*MVP-02:* `run/main_scene` is `res://scenes/menu.tscn` (MVP-19); game scene root `Node2D` (`Main`). F5 → menu → Start.  
*MVP-03:* `RunState` autoload; run RNG single `RandomNumberGenerator` (`reset_run`).  
*MVP-04:* `DamagePipeline` autoload; all damage via `apply_damage` single entry.  
*MVP-05:* `scenes/player.tscn` + WASD movement.  
*MVP-06:* `Camera2D` under player, smoothing.  
*MVP-07:* `enemy_base.tscn` + straight-line AI.  
*MVP-08/16:* `SpawnManager`; wave-based interval and max enemies (`balance.tres`).  
*MVP-09:* Auto-attack + contact damage → `DamagePipeline`.  
*MVP-10:* `run_ended` win/lose.  
*MVP-11/14:* `WaveTimer` + `balance.tres` wave lengths 60/75/90/105/120 s.  
*MVP-12:* Material +2/kill, cap 60, HUD.  
*MVP-13:* Between-wave shop, `shop_open`.  
*MVP-14:* `BalanceData` + `balance.tres` central balance.  
*MVP-15:* `wave_hp_multipliers`, `_scaled_hp()`.  
*MVP-17:* HUD (health bar, wave, material).  
*MVP-18:* `SfxBus` + `assets/sfx/*.wav`.  
*MVP-19:* Menu, pause (`PauseOverlay`), result buttons.  
*MVP-20:* Validation; shop+pause ESC conflict fixed; B table; MVP acceptance.  
*MVP-22:* MVP freeze (no new features, bugfixes only); git tag `mvp-0.1`.

---

## A) MVP build — functional (from `plan_mvp.md`)

| # | Check | Yes | No | Partial | Notes |
|---|--------|-----|-----|---------|-------|
| A1 | Game launches with F5; main flow reachable | Yes | | | MVP-19: menu → Start → game. |
| A2 | Player moves; camera follows | Yes | | | MVP-05–06. |
| A3 | Enemies spawn and pose threat | Yes | | | MVP-08/16. |
| A4 | Auto-attack works (no aiming) | Yes | | | MVP-09. |
| A5 | Damage/death on one coherent path | Yes | | | `DamagePipeline`. |
| A6 | Wave lengths 60 / 75 / 90 / 105 / 120 s | Yes | | | `balance.tres`. |
| A7 | Win after completing 5 waves | Yes | | | `notify_wave_completed(5)`. |
| A8 | Lose on player death | Yes | | | `run_ended(false)`. |
| A9 | Material +2/kill, cap 60 | Yes | | | HUD. |
| A10 | Shop after wave; 30-cost purchase possible | Yes | | | Waves 1–4. |
| A11 | HP scaling ×1.00 … ×1.40 | Yes | | | `_scaled_hp()`. |
| A12 | Spawn pressure increases with wave | Yes | | | 2.2s/8 → 0.9s/35. |
| A13 | No crash/softlock | Yes | | | `shop_open` + pause fix. |

---

## B) MVP build — balance and feel (`mvp_balance_goals.md`)

| # | Check | Yes | No | Partial | Notes |
|---|--------|-----|-----|---------|-------|
| B1 | Run ~7.5 min band | Yes | | | Total 450 s. |
| B2 | Wave curve learn → pressure → climax | | | Partial | Needs playtest sign-off. |
| B3 | Unfair spikes rare | | | Partial | Needs playtest. |
| B4 | Enemy TTK ~1–4 s | Yes | | | ~1–1.5 s. |
| B5 | Rare “nothing to buy” shop walks | | | Partial | Tight on short waves. |
| B6 | Shop options feel meaningful | Yes | | | HP + damage. |
| B7 | Death cause readable | | | Partial | Health bar; no damage numbers. |

---

## C) Demo build — extra bar (`plan_mvp_to_demo.md`)

| # | Check | Yes | No | Partial | Notes |
|---|--------|-----|-----|---------|-------|
| C1 | Main menu + audio/fullscreen | | | Partial | No fullscreen setting. |
| C2 | Result screen | | | Partial | No score/summary. |
| C3 | Shop UI readable | | | Partial | No icons. |
| C4 | SFX | Yes | | | SfxBus. |
| C5 | Music | | | | Not yet. |
| C6 | Low-end FPS | | | | — |
| C7 | Windows export | Yes | | | MVP-21: `build/windows/ProjectA.exe` + smoke; 2026-03-28. |
| C8 | Steam demo flow | | | | — |
| C9 | Store page | | | | — |

---

## D) Decision

- **MVP sign-off:** Critical A rows (A7, A8, A10, A13) = Yes.  
- **Demo sign-off:** Majority of C not Yes after MVP-21.

**Recorded decision:**  
- **MVP accepted** — A complete; B1/B4/B6 Yes; B2/B3/B5/B7 Partial.  
- **Demo not accepted** — C2/C3 Partial; C5–C6 not tested; C7 Yes (MVP-21).

---

## Türkçe

**Ne bu form?** MVP ve Demo için **test kapısı**: A fonksiyonel, B denge/his, C demo çubuğu. Her satırda **Evet / Hayır / Kısmen** işaretle; **not** sütununa kısa gözlem. **MVP onayı** için A7, A8, A10, A13 kritik. Üstteki tabloların güncel metni **İngilizce**dir; build bilgisi ve imzalı karar yukarıda.
