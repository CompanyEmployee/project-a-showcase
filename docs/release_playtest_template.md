# GitHub Release — pre-demo / playtest (copy-paste)

Use when executing [Step 2 in `distribution_plan.md`](distribution_plan.md#step-2--first-playtest--pre-demo-release-when-you-have-a-build).  
Attach your **zipped export** as the release asset (do not commit the zip to `main`).

## Suggested tag

`playtest-0.1` or `pre-demo-YYYY-MM` (pick one scheme and stay consistent).

## Suggested release title

`Pre-demo playtest build (not the Steam demo)`

## Release description (English — paste into GitHub)

```markdown
### What this is

- **Pre-demo / playtest** build of **Project A** (2D roguelite / survivor-like, Godot 4.6.1).
- **Not** the final store demo. The **official demo** will be on **Steam** when available.

### Requirements

- **Windows** (adjust if you ship another platform).
- Extract the zip and run the executable inside.

### Notes

- For feedback, use [Issues](https://github.com/umut-yasin-yilmaz/project-a-showcase/issues) or your preferred channel (link if different).
- No commercial sale; early testing only.

### AI / process

- Development uses **AI as an implementation assistant**; design acceptance is manual. See repository README for workflow context.
```

## Kısa Türkçe not (isteğe bağlı, aynı Release açıklamasının altına)

```markdown

---

**Türkçe:** Bu sürüm **ön-demo / playtest** amaçlıdır; **mağaza demosu değildir**. Resmi demo **Steam**’de yayınlandığında oradan sunulacaktır.
```

## After publish

- If the repo is **public**, anyone with the Releases URL can download.
- If the repo is still **private**, only users with repo access can download—invite testers or share the zip another way.
