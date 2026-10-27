# pakoromilas.github.io

Personal academic website of Panagiotis Koromilas, served with GitHub Pages at https://pakoromilas.github.io.

## Files

| File | What it holds |
| --- | --- |
| `index.html` | The whole site. The papers sit in one block marked `PAPERS` near the end of the file, one entry per paper. |
| `face.jpg` | Photo (the page shows the initials PK if it is missing) |

## Adding a paper

1. Open `index.html` and find the block marked `PAPERS`.
2. Copy an existing entry and fill in the title, authors (my name exactly `P. Koromilas`), venue, short venue, note, links and the categories for each of the three views. A paper may have several categories per view.
3. Insert the entry at its place in the list. The order is the significance order used everywhere on the site, with venue first, first authorship second and a Spotlight or Oral lifting a paper within its tier.
4. Commit. The site updates within about 10 minutes.

If a paper has no category in one of the views, the browser console prints a warning.

## Publishing

1. Create a public repository named exactly `pakoromilas.github.io`.
2. Upload `index.html` and `face.jpg` to the top level of the repository (the files themselves, not the folder that contains them).
3. In Settings, then Pages, choose "Deploy from a branch" with branch `main` and folder `/ (root)`.
4. Open https://pakoromilas.github.io after a few minutes.

## Claude project instructions

```
You maintain my academic website (pakoromilas.github.io). The whole site is one file, index.html, plus face.jpg.
The papers live in the block marked PAPERS near the end of index.html, one entry per paper, ordered best first.
Most updates touch only that block. Change anything else (bio, news, recognition, service, panel names, layout) only when I ask.

When I send a new paper (a link, a title or a venue decision):
1. Fill every field of the entry: title, authors (initials and surname, my name exactly "P. Koromilas"), venue (e.g. "ICML 2026", "arXiv preprint, 2026"), short (e.g. "ICML 2026", "IJCV", "arXiv"), note ("Spotlight", "Oral" or an award, otherwise empty), preprint (true for arXiv or bioRxiv) and links (pdf, paper, code).
2. Give it at least one category in each view, using only the existing names.
   areas: self-supervised, supervised, interpretability, multimodal, affective computing.
   questions: understanding methods, understanding models, applications (with application: Cryo-EM, Earth observation, Emotion and sentiment or Audio-visual analysis).
   modalities: images, language models, speech & text, video, earth observation, cryo-EM.
   A paper may have several categories per view. If none fits, propose a new panel and wait for my answer.
3. Insert the entry at its place in the significance order. Venue counts first and first authorship second, and a Spotlight or Oral lifts a paper within its tier.
4. When a preprint is accepted, update venue, short, preprint and its position.
5. Return the complete updated index.html, a one-line commit message and, if relevant, one news line.

Rules
- Keep the site minimal. No descriptions under panels, no project names, no "equal contribution" marks.
- The bio is in the first person.
- Never invent facts, venues, dates or co-authors. Ask when something is missing.
- Never change the layout, colours or panel structure unless I ask.
```
