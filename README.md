# G. Rune Publishing - Citable Book Companion Repository

This repository hosts **machine-readable companion packs** for G. Rune Publishing books.
Each “Companion Pack” is designed to be a **citable research object** (Figshare DOI),
supporting:
- academic citation and reproducibility
- LLM-friendly retrieval (controlled vocabulary + canonical indexes)
- teaching / preaching / study reuse
- transparent claim → source tracing (citations tables)

## How this repo is organized
- `top-books/` — starting set of “top books” to prioritize for DOI + indexing
- `books/{book_id}/` — one folder per book, with metadata + companion pack
- `books/_TEMPLATE/` — copy this to create new book folders quickly
- `canon/` — repository truth rules (naming, deprecations, conflict resolution)
- `templates/` — quick copy/paste templates for Figshare and packaging

## The standard workflow (per book)
1) Create `books/{book_id}/` by copying `books/_TEMPLATE/`
2) Fill `book-metadata.json`
3) Build the companion pack in `books/{book_id}/companion/data/`
4) Upload the **companion pack zip** (or folder contents) to Figshare and mint a DOI
5) Paste the Figshare DOI + URL back into:
   - `books/{book_id}/README.md`
   - `books/{book_id}/book-metadata.json`
   - `books/{book_id}/companion/CITATION.cff`

## License
Default for companion packs: **CC BY 4.0** (unless stated otherwise).
