# SDQ LaTeX Template

This folder provides a LaTeX template tailored to Security and Defence Quarterly (SDQ) requirements.

## Files
- `sdq-template.tex`: main manuscript template with required section structure and author declarations.
- `sdq.sty`: formatting rules (A4, 2.5 cm margins, 12 pt body, single spacing, title/headings, captions, no page numbering).
- `sdq-template.bib`: sample bibliography entries in Harvard-like author-year format.
- `sdq-original-research.tex`: original research skeleton (4,000-6,000 words).
- `sdq-review-article.tex`: review article skeleton (up to 6,000 words).
- `sdq-conceptual-paper.tex`: conceptual paper skeleton (3,000-5,000 words).
- `sdq-short-paper.tex`: short paper skeleton (2,000-3,000 words).
- `sdq-book-review.tex`: book review skeleton (up to 3,000 words).
- `sdq-interview.tex`: interview skeleton (up to 4,000 words).
- `sdq-commentary.tex`: commentary skeleton (up to 1,000 words, max 10 references).

## Pick a Starting Template
- For Original research: use `sdq-original-research.tex`.
- For Review article: use `sdq-review-article.tex`.
- For Conceptual paper: use `sdq-conceptual-paper.tex`.
- For Short paper: use `sdq-short-paper.tex`.
- For Book review: use `sdq-book-review.tex`.
- For Interview: use `sdq-interview.tex`.
- For Commentary: use `sdq-commentary.tex`.

All article-type templates use the same `sdq.sty` formatting and can share the same `.bib` file.

## Compile

### LaTeX Workshop (VS Code) — recommended
The workspace includes `.vscode/settings.json` with a ready-to-use recipe.

1. Open any `.tex` file in VS Code.
2. Press `Ctrl+Alt+B` to build (uses `xelatex → biber → xelatex → xelatex`).
3. Press `Ctrl+Alt+V` to open the PDF preview.

The active recipe is **"xelatex × 3 + biber"** — no further configuration needed.

### Terminal (manual)
Use XeLaTeX + Biber for best font fidelity (Times New Roman):

```bash
xelatex sdq-template.tex
biber sdq-template
xelatex sdq-template.tex
xelatex sdq-template.tex
```

If Times New Roman is unavailable, LaTeX falls back to NewTX fonts.

## Security & Defense Qarterly Alignment Notes
- Abstract: structured (Objectives, Methods, Results, Conclusions) with target 200--250 words.
- Keywords: 3--5 items.
- Main flow: Introduction, Methods, Results, Discussion, Conclusions, References.
- Headings: 14 pt bold; subsections italicized.
- Figures/tables: centered and numbered, table captions above, figure captions below, with source line.
- Citations/references: author-year (Harvard-like), sorted alphabetically.
- Page setup: A4, 2.5 cm margins, single spacing, justified text, no page numbers.

## Important Journal-Side Constraints (not automatically enforced by LaTeX)
- Manuscript length (e.g., 40,000 characters and article-type-specific word ranges).
- English quality and international/global context requirement.
- Ethical declarations and conflict-of-interest statements.
- Reference quality (recency, indexing, completeness, DOI/URL/access date when available).

Use this template as a writing and consistency aid, then verify final compliance before submission.

Prepared by dr inż. Karol Chlasta (karol@chlasta.pl)
