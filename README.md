# Project A — Public showcase

Vitrin deposu: **Project A**’nın **MVP (`mvp-0.1`)** ile uyumlu, herkese açık özet.  
Asıl geliştirme ve ticari içerik **private** repoda kalır.

![Project A MVP showcase banner](assets/showcase/hero-mvp.svg)

**Bu sayfa hangi sürümü temsil ediyor?** Public özet ve görseller **MVP milestone** (`mvp-0.1`, private repoda `MVP-01` → `MVP-22`) ile hizalıdır; canlı üretim kodu ve assetler burada yoktur.

---

## Şimdi · Sırada

| Şimdi | Sırada (public vitrin) |
|--------|-------------------------|
| MVP tamamlandı; bu repo süreç + yön + güvenli dokümanlarla hizalı | Demo / mağaza yüzüne uygun ek görseller veya kısa gameplay kaydı (isteğe bağlı) |
| README ve `docs/` ile portfolio/recruiting için okunabilir kanıt | İleride Itch / Steam bağlantıları bu vitrine eklenebilir |

---

## Oyun özeti

**Project A**, Brotato tarzı tempolu **2D roguelite / survivor-like** bir yapım.

**Çekirdek döngü**
- Zamanlı dalgalarda düşmanlarla savaş
- Düşen materyalleri topla
- Dalgalar arası yükseltme satın al
- Koşuyu sonuna kadar taşı

### Gösterim medyası (isteğe bağlı)

Gerçek oyun görüntüsü eklemek için `assets/showcase/` klasörüne bakın. Önerilen dosya adları: `mvp-gameplay.gif`, `mvp-01-wave.png`, … — ayrıntı: [assets/showcase/README.md](assets/showcase/README.md).

---

## Shipped MVP (showcase görünümü)

- **Motor:** Godot 4.6.1  
- **Dil:** Typed GDScript (production)  
- **Hedef:** PC (Steam-first)  
- **Model:** AI destekli solo geliştirme; kabul kriterleri ve tasarım öncelikleri manuel  
- **Public amaç:** Kaynak sızdırmadan süreç kalitesi ve milestone disiplinini göstermek  

---

## Bu reponun amacı

- Tasarım yönü ve MVP sınırları  
- Planlama ve QA / risk disiplini  
- **Tamamlanmış MVP** bağlamında portfolio/recruiting için güvenli kanıt  

## Süreç özeti (AI destekli solo)

- Blueprint ve açık **non-goals** ile kapsam kontrolü  
- MVP / demo yol haritası ve kapanış kriterleri  
- Milestone öncesi **QA checklist** kapıları  
- Tekrarlayan riskler için **risk register**  
- Küçük, niyeti net checkpoint commit’leri  

---

## Önerilen okuma sırası (`docs/`)

1. [`docs/blueprint.md`](docs/blueprint.md) — pitch, oturum hedefi, çekirdek döngü  
2. [`docs/qa_checklist.md`](docs/qa_checklist.md) — milestone test kapıları  
3. [`docs/risk_register.md`](docs/risk_register.md) — üretim riskleri  

---

## Public / private sınırı

**Bu repoda bilerek olanlar:** vizyon, üst seviye oyun hedefleri, MVP bağlamı, üretim sırlarına girmeyen süreç dokümanları.  

**Private repoda kalanlar:** tam oyun kaynağı ve mimari iç detaylar, ticari sanat/ses ve pipeline, ince ayar/balance ve dağıtıma dair hassas bilgiler, gizli kimlik bilgileri.  

---

## Neden bu strateji?

Ticari indie üretim için: **koruma** (ana içerik private), **görünürlük** (tutarlı public vitrin), **güvenilirlik** (net milestone ve süreç).  

---

## Status

**MVP** private ana repoda **`mvp-0.1`** ile tamamlandı. Bu showcase, aynı milestone ile uyumlu **güvenli, vitrin** içeriği sunar.

---

## English (short)

Public-facing showcase for **Project A** (2D roguelite / survivor-like, Godot 4.6.1). **MVP shipped** as tag `mvp-0.1` in the private dev repo. This repository contains **no full source or commercial assets**—only safe process docs and optional media you add under `assets/showcase/`. Main development stays private.

**Suggested doc order:** [blueprint](docs/blueprint.md) → [QA checklist](docs/qa_checklist.md) → [risk register](docs/risk_register.md).
