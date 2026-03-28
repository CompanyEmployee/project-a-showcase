# Godot export → zip → GitHub Release (Project A)

Use this when publishing a **playtest** build to **`project-a-showcase` Releases**.  
Do **not** commit the zip or `build/` folder to git (`project-a` already ignores `/build/`).

## 1. Export in Godot (private `project-a`)

1. Open the project in **Godot 4.6.x** (same major/minor as production).
2. **Project → Export…**
3. Select preset **Windows Desktop** (defined in `export_presets.cfg`; export path is `build/windows/ProjectA.exe`).
4. If you have not installed export templates yet, Godot will prompt you — install **matching** templates.
5. Click **Export Project**, confirm path `build/windows/ProjectA.exe` (Godot will create the `build/windows/` folder if needed).
6. After export, open **`build/windows/`** on disk and confirm:
   - `ProjectA.exe` is present
   - Any **`.pck`** or **`.dll`** / **`.so`** files Godot generated sit **next to** the exe (with `embed_pck` off, a `.pck` is required alongside the exe).

## 2. Zip the folder (not the repo root)

1. Zip **everything inside** `build/windows/` (exe + pck + other files), **or** zip the `windows` folder as a single unit.
2. Name example: `ProjectA-windows-playtest-01.zip` (avoid spaces if you like cleaner URLs).

**Do not** put the zip under `project-a-showcase` git tree and commit it — only attach it to a **Release**.

## 3. Create a GitHub Release (`project-a-showcase`)

1. On GitHub open **`umut-yasin-yilmaz/project-a-showcase`**.
2. **Releases** → **Draft a new release**.
3. **Choose a tag:** create new tag, e.g. `playtest-0.1` or `build-2026-03-28` (must not duplicate an existing tag).
4. **Release title:** short, e.g. `Windows playtest build`.
5. **Description:** copy from [`release_playtest_template.md`](release_playtest_template.md) and adjust version / notes.
6. **Attach binaries:** drag your zip under **Attach binaries**.
7. **Publish release**.

## 4. While the repo is **private**

Only GitHub users **with access** to `project-a-showcase` can see Releases and download the zip. Invite collaborators under **Settings → Collaborators** if needed, or share the zip outside GitHub.

## 5. After the repo goes **public**

The same Release page becomes visible to everyone; you can add a line in the root README pointing to **Releases** for the latest zip.
