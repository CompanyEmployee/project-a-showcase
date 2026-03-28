# Distribution plan (Project A showcase)

This file is the **step-by-step** companion to the [Downloads & distribution](../README.md#downloads--distribution) section in the root README.

## Showcase repo visibility (planned lifecycle)

1. **Curation phase (now):** Keep the showcase repo **private** while you polish README, screenshots, and `docs/`—so work-in-progress is not publicly visible.
2. **When the vitrin is ready:** Set the repo back to **public**:
   - **GitHub web:** Repository **Settings** → **Danger zone** → **Change repository visibility** → **Public**, or  
   - **CLI:** `gh repo edit umut-yasin-yilmaz/project-a-showcase --visibility public --accept-visibility-change-consequences`
3. **After it is public:** Pin **project-a-showcase** on your profile (then **everyone** can see the pin and the repo). Optionally set **bio** / **website** to the showcase or future store link.

While the repo is **private**, only you and collaborators can read the README and download **Releases**.

## Step 0 — Baseline

- Private dev repo: source of truth, regular push, milestone tags.
- Showcase repo: **private during curation**; content target is EN + TR README, screenshots, `docs/` (blueprint, QA, risk), boundaries documented—then **public** again (see lifecycle above).

## Step 0.5 — Flip showcase to public (when vitrin is finalized)

Do this **once** you are happy with the showcase content (no more half-finished edits you care about hiding):

0. Optional gate: walk [`docs/before_public_checklist.md`](before_public_checklist.md).
1. Run the visibility change (web UI or `gh repo edit ... --visibility public --accept-visibility-change-consequences`).
2. Quick pass: open the repo in a **logged-out** browser or incognito to confirm README and default branch look correct.
3. Continue with **Step 1** (pin + bio/website).

## Step 1 — GitHub profile (after showcase is public)

- **Pin** `project-a-showcase` on your GitHub profile (visible to visitors once the repo is public). Click-by-click: [`docs/step1_pin_profile.md`](step1_pin_profile.md).
- Optionally set **bio** and **website** (showcase URL, later Steam/Itch).

**While the showcase is still private:** pinning helps only you on your profile; defer the “portfolio pin” until **Step 0.5** is done.

## Step 2 — Playtest Release (Godot export → zip → GitHub)

Detailed steps: [`docs/godot_export_and_release.md`](godot_export_and_release.md).

1. In **private** `project-a`, export **Windows Desktop** (preset → `build/windows/ProjectA.exe`).
2. Zip the **`build/windows/`** output (exe + `.pck` and any DLLs together). **Do not** commit the zip to either repo’s `main`.
3. On GitHub: **project-a-showcase** → **Releases** → **Draft a new release**.
4. Create a new tag, e.g. `playtest-0.1` or `build-2026-03-28`.
5. Title example: `Windows playtest build`.
6. Description: [`docs/release_playtest_template.md`](release_playtest_template.md).
7. Attach the zip → **Publish**.

**Note:** While the showcase repo is **private**, only users **with access** can download. After **public**, the same Release is visible to everyone.

## Step 3 — After a store demo exists (later)

*Skip until you actually ship a store demo (e.g. Steam).*

1. Update showcase **README** → **Downloads & distribution** with an **official** demo/store link if you want one canonical URL.
2. **Remove or archive** obsolete GitHub Release playtest assets if needed.
3. Refresh any download wording so it matches reality.

## Step 4 — Store compliance

- **Steam:** Fill **AI disclosure** (and other required fields) per [current Steamworks rules](https://partner.steamgames.com/) when you publish the store page.
- Keep a short **credits** note (Godot MIT, third-party assets if any).

## Step 5 — Optional automation (later)

- Godot export via **GitHub Actions** and/or upload to **Itch** with **butler**—only if you want CI; not required for the manual path above.

---

Check off steps in your own tracker; update this file if your tag naming or platforms change.
