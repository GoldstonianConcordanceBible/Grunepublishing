# SOP — Copy/Paste Template Setup (Series Publishing Hub)

This SOP explains exactly how to create and reuse the publishing template for a 5-book series inside this repo.

---

## A) Where this series lives (required)
All files for this series live at:

`series/the-testimony-of-dr-justin-goldston/`

Do NOT put these in root. Keep them inside `series/`.

---

## B) Folder creation steps (exact order)

### 1) Create these folders
Create each folder exactly as written:

- `series/`
- `series/the-testimony-of-dr-justin-goldston/`
- `series/the-testimony-of-dr-justin-goldston/books/`
- `series/the-testimony-of-dr-justin-goldston/books/01-for-sydney/`
- `series/the-testimony-of-dr-justin-goldston/books/02-wrestling-with-god/`
- `series/the-testimony-of-dr-justin-goldston/books/03-the-devil-knows-the-bible-too/`
- `series/the-testimony-of-dr-justin-goldston/books/04-the-devils-doctrine-of-distraction/`
- `series/the-testimony-of-dr-justin-goldston/books/05-the-faith-hacker/`

---

## C) File creation steps (what files go where)

### 2) Create these series-level files (inside the series folder)
Create these files:

- `series/the-testimony-of-dr-justin-goldston/README.md`
- `series/the-testimony-of-dr-justin-goldston/DISCLAIMER.md`
- `series/the-testimony-of-dr-justin-goldston/PRIVACY-AND-NAMES.md`
- `series/the-testimony-of-dr-justin-goldston/SERIES-OVERVIEW.md`
- `series/the-testimony-of-dr-justin-goldston/SOP-COPY-PASTE.md` (this file)

### 3) Create this books index file (inside the books folder)
Create this file:

- `series/the-testimony-of-dr-justin-goldston/books/README.md`

### 4) Create these 3 files inside EACH book folder
Each book folder must contain:

- `README.md`
- `amazon-description.md`
- `keywords.md`

Example for Book 1:
- `series/the-testimony-of-dr-justin-goldston/books/01-for-sydney/README.md`
- `series/the-testimony-of-dr-justin-goldston/books/01-for-sydney/amazon-description.md`
- `series/the-testimony-of-dr-justin-goldston/books/01-for-sydney/keywords.md`

Repeat for books 02–05.

---

## D) How to reuse this template for a NEW series (copy/paste method)

### 5) Duplicate the whole series folder
Copy this folder:

`series/the-testimony-of-dr-justin-goldston/`

Paste it as a new folder name, example:

`series/<new-series-slug>/`

A “slug” is lowercase with hyphens. Example:
- `series/faith-hackers-kids/`
- `series/goldstonian-legacy-dossier/`

### 6) Update the series-level files
Open and edit ONLY these fields:
- In `README.md` change the series title
- In `SERIES-OVERVIEW.md` change the overview text
- Keep `DISCLAIMER.md` and `PRIVACY-AND-NAMES.md` unless the new series needs different privacy rules

### 7) Update each book folder name + headings
Rename:
- `books/01-...` etc. to match your new titles

Then update:
- Each book `README.md` title line
- Each book `amazon-description.md`
- Each book `keywords.md`

---

## E) Naming rules (so it stays consistent)

### 8) Folder naming rule (required)
- Use lowercase
- Use hyphens
- No punctuation

Correct:
- `the-devil-knows-the-bible-too`
Wrong:
- `The Devil Knows The Bible Too`

### 9) Book ordering rule (required)
Always use two-digit numbers:
- `01-`
- `02-`
- `03-`
- `04-`
- `05-`

This keeps books in the right order in GitHub.

---

## F) Publishing usage (what each file is for)

### 10) What to do with the files
- `amazon-description.md` → copy into your Amazon “Book Description” field
- `keywords.md` → copy into your keyword planning + metadata work (and keep it here as your master)
- `DISCLAIMER.md` + `PRIVACY-AND-NAMES.md` → keep public-facing for safety and clarity
- `SERIES-OVERVIEW.md` → use for the series page, press kit text, and YouTube/podcast descriptions

---

## G) Commit procedure (simple)

### 11) Commit message template
When you add or update the series folder, use one of these commit messages:

- `Add testimony series publishing hub template`
- `Update series overview + book metadata`
- `Add book descriptions + keywords`

---

## H) Zero-evidence rule (important)
This repo folder is for publishing language only.
Do NOT upload private records, screenshots, messages, or anything involving a minor’s private info.

Keep testimony public. Keep evidence private.