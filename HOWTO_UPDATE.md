# How to Update This Website

## 1) Add a New Publication

1. Add a new BibTeX entry to `assets/bibliography/references.bib`.
2. Create a new folder under `content/publications/` with a slug, for example `content/publications/my-new-paper/`.
3. Add `content/publications/my-new-paper/index.md` with metadata (`title`, `authors`, `date`, `publication_types`, `publication`, `abstract`, `summary`).
4. Add `content/publications/my-new-paper/cite.bib` with the BibTeX entry for the Cite popup button.

## 2) Update Biography

Primary biography text is in `content/authors/admin/_index.md`.

For the resume blocks on the homepage, keep `data/authors/admin.yaml` in sync for:
- `role`
- `bio`
- `affiliations`
- `links`
- `education`
- `experience`

## 3) Add a Talk

1. Create a folder under `content/events/`, for example `content/events/my-new-talk/`.
2. Add `index.md` with:
   - `title`
   - `date`
   - `event_name`
   - `location`
   - `summary`
   - `abstract`
   - `event_start` and `event_end`

## 4) Local Preview Before Pushing

From the repo root:

```bash
npm install
hugo server
```

Then open `http://localhost:1313/` and verify:
- bio and contact links
- publication cards and Cite buttons
- talks/news cards
- no blog/projects/courses sections in navigation
