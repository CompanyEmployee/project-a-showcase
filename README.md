# Project A Showcase

Curated showcase for **Project A**.

**Visibility (maintainer intent):** This repository is **temporarily private** while the showcase (README, screenshots, docs) is being refined—so incomplete edits are not visible to the world. **When the vitrin is finalized, it will be set back to public** for portfolio and discovery. The main development repository stays **private**.

While private: only you—and anyone you grant access—can read this README and Releases.

**Milestone:** **MVP shipped** — `MVP-01` → `MVP-22` complete in the private repo; Git tag **`mvp-0.1`**.  
**Current focus:** Demo / portfolio-facing updates (screenshots, README, safe docs) while keeping source and assets out of this narrative layer.

**This README reflects the MVP (`mvp-0.1`) build** as a safe vitrin layer: no full source or commercial assets here—only curated docs and screenshots.

## MVP build snapshots

Screenshots from the current MVP build:

| | | |
| :---: | :---: | :---: |
| ![MVP gameplay snapshot 1](assets/showcase/mvp-screenshot-01.png) | ![MVP gameplay snapshot 2](assets/showcase/mvp-screenshot-02.png) | ![MVP gameplay snapshot 3](assets/showcase/mvp-screenshot-03.png) |

## Overview

Project A is a 2D roguelite/survivor-like game inspired by Brotato-style pacing.

Core loop:

- Fight enemies in timed waves
- Collect materials from defeated enemies
- Buy upgrades between waves
- Survive the full run

## Shipped MVP (showcase view)

- Engine: Godot 4.6.1
- Language: Typed GDScript (production)
- Target platform: PC (Steam-first)
- Development model: AI-assisted solo developer workflow
- Showcase objective: demonstrate process quality, shipped MVP discipline, and direction safely (no full source here)

## Showcase repository purpose

This repository is intentionally curated to show:

- Design direction and MVP boundaries
- Development discipline and planning quality
- Progress and **milestone completion** suitable for portfolio/recruiting

## Professional Workflow

Project A follows a structured production workflow:

- Scope control through blueprint and explicit non-goals
- MVP and Demo roadmap with completion criteria
- QA checklist gates before milestone closure
- Risk register tracking for recurring production risks
- Small, checkpoint-style updates with clear intent

## Documents in this repository

- [`docs/blueprint.md`](docs/blueprint.md) (project pitch, target session, core loop)
- [`docs/qa_checklist.md`](docs/qa_checklist.md) (test gate checklist)
- [`docs/risk_register.md`](docs/risk_register.md) (production risk tracking)
- [`docs/distribution_plan.md`](docs/distribution_plan.md) (distribution steps overview)
- [`docs/before_public_checklist.md`](docs/before_public_checklist.md) (before setting repo public)
- [`docs/step1_pin_profile.md`](docs/step1_pin_profile.md) (after repo is public)
- [`docs/release_playtest_template.md`](docs/release_playtest_template.md) (playtest Release copy-paste)
- [`docs/godot_export_and_release.md`](docs/godot_export_and_release.md) (Godot → zip → GitHub Release)

**Suggested reading order:** blueprint → QA checklist → risk register.

Workflow note:

- AI is used as an implementation and iteration assistant.
- Final design priorities and acceptance criteria are reviewed manually.

## Boundary: this repo vs dev repo

### Curated in this showcase repository

- Project vision and high-level gameplay goals
- Safe progress updates and **MVP-shipped** milestone context
- Process artifacts that do not expose production internals

### Stays in the private dev repository only

- Full gameplay source code and architecture internals
- Commercial art/audio assets and content pipeline
- Implementation-level balance/tuning and deployment details
- Any secrets, credentials, or release-sensitive information

## Why this strategy

For a commercial indie project, this setup balances:

- **Protection:** main production content stays private
- **Controlled curation:** private while polishing the vitrin; then **public** again for normal showcase visibility
- **Credibility:** clear workflow and milestone-based execution

## Status

**MVP is complete** in the private main repository (`mvp-0.1`).  
This showcase repo is updated with **safe, portfolio-ready** context aligned with that milestone.

## Downloads & distribution

- **Source of truth for code/assets:** the **private** dev repo. This showcase repo does **not** host source on `main`.
- **Playtest builds:** **Windows** exports from Godot are shipped as **GitHub Release** attachments (zip), **not** committed to git. Full workflow: [`docs/godot_export_and_release.md`](docs/godot_export_and_release.md). Release notes template: [`docs/release_playtest_template.md`](docs/release_playtest_template.md).
- **While this repo is private:** only accounts **with access** can see Releases and download zips (invite collaborators if needed).
- **When this repo is public:** the same Releases page becomes world-visible; you can add a one-line pointer here to the latest Release.
- **Principle:** These zips are **non-commercial** playtest drops. Store-facing demo pages (e.g. Steam) are **out of scope** for this README until that phase is real—then this section can be updated.

Maintainer checklist: [`docs/distribution_plan.md`](docs/distribution_plan.md).  
Before switching this repo to **public:** [`docs/before_public_checklist.md`](docs/before_public_checklist.md).

---

## Türkçe vitrin

**Project A** için vitrin deposu.

**Görünürlük (bakım notu):** Repo şu an **geçici olarak private** — vitrin (README, görseller, dokümanlar) oturtulurken yarım kalmış değişikliklerin herkese açık görünmesini engellemek için. **Vitrin hedef haline gelince repo tekrar public yapılacak.** Asıl geliştirme deposu ticari içerik için **private** kalmaya devam eder.

Private iken: README ve Releases’i yalnızca sen ve erişim verdiğin hesaplar görür.

**Milestone:** **MVP tamamlandı** — private repoda `MVP-01` → `MVP-22`; Git etiketi **`mvp-0.1`**.  
**Güncel odak:** Kaynak ve assetleri ayrı tutarken demo / portfolio odaklı güncellemeler (ekran görüntüleri, README, güvenli dokümanlar).

**Bu README, MVP (`mvp-0.1`) sürümünü** güvenli bir vitrin katmanı olarak özetler (tam kaynak veya ticari asset yok; seçilmiş doküman ve görseller var).

### MVP sürümünden ekran görüntüleri

| | | |
| :---: | :---: | :---: |
| ![MVP oyun görüntüsü 1](assets/showcase/mvp-screenshot-01.png) | ![MVP oyun görüntüsü 2](assets/showcase/mvp-screenshot-02.png) | ![MVP oyun görüntüsü 3](assets/showcase/mvp-screenshot-03.png) |

### Genel bakış

**Project A**, Brotato tarzı tempolu bir **2D roguelite / survivor-like** yapımdır.

**Çekirdek döngü**

- Zamanlı dalgalarda düşmanlarla savaş
- Yenilen düşmanlardan materyal topla
- Dalgalar arası yükseltme satın al
- Koşuyu sonuna kadar taşı

### Tamamlanan MVP (vitrin özeti)

- **Motor:** Godot 4.6.1
- **Dil:** Typed GDScript (production)
- **Hedef platform:** PC (Steam-first)
- **Geliştirme modeli:** AI destekli solo geliştirici süreci
- **Vitrin amacı:** Kaynak sızdırmadan süreç kalitesi, MVP disiplini ve yönü güvenli şekilde göstermek

### Bu reponun amacı

- Tasarım yönü ve MVP sınırları
- Geliştirme disiplini ve planlama kalitesi
- Portfolio / iş görüşmesi için uygun **milestone tamamlanması** kanıtı

### Profesyonel süreç

- Blueprint ve açık **non-goals** ile kapsam kontrolü
- MVP ve Demo yol haritası + kapanış kriterleri
- Milestone kapanışından önce **QA checklist** kapıları
- Tekrarlayan üretim riskleri için **risk register**
- Niyeti net, küçük checkpoint güncellemeleri

### Bu repodaki dokümanlar

- [`docs/blueprint.md`](docs/blueprint.md) — pitch, oturum hedefi, çekirdek döngü
- [`docs/qa_checklist.md`](docs/qa_checklist.md) — test kapısı checklist
- [`docs/risk_register.md`](docs/risk_register.md) — üretim risk takibi
- [`docs/distribution_plan.md`](docs/distribution_plan.md) — dağıtım adımları (genel)
- [`docs/godot_export_and_release.md`](docs/godot_export_and_release.md) — Godot → zip → Release
- [`docs/before_public_checklist.md`](docs/before_public_checklist.md) — public yapmadan önce kontrol
- [`docs/step1_pin_profile.md`](docs/step1_pin_profile.md) — repo public olduktan sonra pin
- [`docs/release_playtest_template.md`](docs/release_playtest_template.md) — playtest Release metin şablonu

**Önerilen okuma sırası:** blueprint → QA checklist → risk register.

**Süreç notu:** AI uygulama ve iterasyon asistanı olarak kullanılır; tasarım öncelikleri ve kabul kriterleri manuel gözden geçirilir.

### Sınır: bu repo vs geliştirme reposu

**Bu vitrin reposunda bilerek olanlar:** vizyon, üst seviye oyun hedefleri, MVP bağlamı, üretim içine sızmayan süreç dokümanları.

**Yalnızca private geliştirme reposunda kalanlar:** tam oyun kaynağı ve mimari iç detaylar, ticari sanat/ses ve pipeline, implementasyon düzeyinde balance/ince ayar ve dağıtım detayları, gizli bilgiler.

### Neden bu strateji?

Ticari indie üretim için: **koruma** (ana içerik private), **kontrollü vitrin** (hazırlık sürecinde private; hazır olunca tekrar public), **güvenilirlik** (net süreç ve milestone).

### Durum

**MVP**, private ana repoda **`mvp-0.1`** ile tamamlandı. Bu vitrin deposu, aynı milestone ile hizalı **güvenli, portfolio** içeriği sunar.

### İndirmeler ve dağıtım

- **Kod / asset kaynağı:** **private** geliştirme deposu. Bu showcase’in `main` dalında kaynak yok.
- **Playtest build:** Godot **Windows** export’u **GitHub Releases** üzerinde **zip** olarak paylaşılır; zip **`git` ile commit edilmez**. Adımlar: [`docs/godot_export_and_release.md`](docs/godot_export_and_release.md). Release metni şablonu: [`docs/release_playtest_template.md`](docs/release_playtest_template.md).
- **Repo private iken:** Release’leri yalnızca **erişimi olan** hesaplar indirebilir (testçi için Collaborators).
- **Repo public olunca:** Aynı Release sayfası herkese açılır; isteğe bağlı olarak README’ye “son sürüm” satırı eklenebilir.
- **İlke:** Zip’ler **ticari olmayan** playtest içindir. Mağaza demosu / Steam sayfası gibi konular bu README’de **şimdilik yok**; o aşama gerçekten gelince metin güncellenir.

Adım adım kontrol listesi: [`docs/distribution_plan.md`](docs/distribution_plan.md).  
Repoyu tekrar **public** yapmadan önce: [`docs/before_public_checklist.md`](docs/before_public_checklist.md).
