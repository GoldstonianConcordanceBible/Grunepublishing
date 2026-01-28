# MIGRATION-CHECKLIST — Fix Double `series/series/` Path Later

## Goal
Move this series from the current location:

- CURRENT (canonical for now): `series/series/the-testimony-of-dr-justin-goldston/`

to the long-term canonical location:

- TARGET: `series/the-testimony-of-dr-justin-goldston/`

Without duplicating content or breaking links.

---

## Rules (do not skip)
- Do NOT create two “live” copies. After migration, the old path must contain only a redirect note.
- Copy first, verify second, redirect third, then optionally delete old content last.
- Keep folder names identical inside the series folder (books/, agents/, etc.).

---

## Pre-Migration Checklist (before you copy)
1) Confirm CURRENT path exists and is complete:
   - `series/series/the-testimony-of-dr-justin-goldston/README.md`
   - `series/series/the-testimony-of-dr-justin-goldston/books/`
   - All 5 book folders exist: `01-` through `05-`

2) Freeze edits (recommended):
   - Make no edits during the copy/verify step.

3) Search for references to the CURRENT path (record results):
   - Find text: `series/series/the-testimony-of-dr-justin-goldston`
   - Find text: `series/the-testimony-of-dr-justin-goldston`
   Note where each appears so you can update later.

---

## Migration Steps (copy → verify → redirect)
### Step 1 — Create TARGET folder
Create:
- `series/the-testimony-of-dr-justin-goldston/`

### Step 2 — Copy everything from CURRENT to TARGET
Copy the entire folder:
- From: `series/series/the-testimony-of-dr-justin-goldston/`
- To:   `series/the-testimony-of-dr-justin-goldston/`

This includes:
- `books/`
- any series-level files (DISCLAIMER, PRIVACY, OVERVIEW, SOP, etc.)
- any agent packs if stored inside this series folder

### Step 3 — Verify TARGET is complete
Verify in TARGET:
- `series/the-testimony-of-dr-justin-goldston/books/01-for-sydney/`
- `series/the-testimony-of-dr-justin-goldston/books/02-wrestling-with-god/`
- `series/the-testimony-of-dr-justin-goldston/books/03-the-devil-knows-the-bible-too/`
- `series/the-testimony-of-dr-justin-goldston/books/04-the-devils-doctrine-of-distraction/`
- `series/the-testimony-of-dr-justin-goldston/books/05-the-faith-hacker/`

Each book folder must contain:
- `README.md`
- `amazon-description.md`
- `keywords.md`

### Step 4 — Update repo indexes (only after TARGET verified)
Update links that point to the CURRENT path.

Minimum places to check/update:
- Repo root `README.md`
- `series/README.md` (if present)
- `catalog/` files (if they reference this series path)
- `canon/` files (if they reference this series path)
- `agents/AGENTS-INDEX.md` (if it links into series content)
- Any “top-books” or curated lists

Replace:
- `series/series/the-testimony-of-dr-justin-goldston`
with:
- `series/the-testimony-of-dr-justin-goldston`

### Step 5 — Convert CURRENT folder into a redirect (do not delete yet)
In CURRENT path, delete/move all contents ONLY after you’ve verified the TARGET is correct.

Then leave behind ONLY:
- `README.md` (redirect note)
- This file: `MIGRATION-CHECKLIST.md` (optional to keep)
- Any deprecation notice files you want to keep

Redirect README content:
- “Moved to /series/the-testimony-of-dr-justin-goldston/”

### Step 6 — Final verification (no broken navigation)
- Click from repo root → series → testimony series
- Confirm it opens TARGET path
- Confirm each book folder opens in TARGET path
- Confirm no curated lists point to CURRENT path

---

## Optional Cleanup (later, after everything works)
- Delete CURRENT folder contents except redirect README.
- If you keep redirect forever, that’s fine.

---

## Commit Plan (safe commits)
Suggested commit sequence:
1) `Create migration target path for testimony series`
2) `Copy testimony series to canonical series/ path`
3) `Update references to canonical testimony series path`
4) `Add redirect note at old series/series/ path`

---

## “Done” Definition
Migration is complete when:
- TARGET exists and contains the full series
- All references in repo point to TARGET
- CURRENT contains only a redirect note (no duplicate content)