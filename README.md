# One-page Tailwind Resume + Cover Letter (Finland-ready)

Static, single-page resume and cover letter that read data from JSON files, print cleanly on A4, and deploy easily to GitHub Pages.

## How to use
1) Edit your content in `resume-playbook.md` (source of truth) and mirror updates into `data/resume.json`.
2) Open `index.html` for resume preview and `cover-letter.html` for cover letter preview.
3) Edit `data/resume.json` for CV content and `data/cover-letter.json` for letter content.
4) For each application, tailor `basics.summary` and bullets in `data/resume.json`, then update recipient/subject/paragraphs in `data/cover-letter.json`.
5) Print or save to PDF via the **Print / Save PDF** button. In the print dialog pick **A4**, scale 100%, and uncheck headers/footers.

## GitHub Pages deployment
1) Commit all files to your repo.
2) In GitHub: Settings → Pages → Build and deployment → Source = `Deploy from a branch`; Branch = `main` (or default) `/root`.
3) Wait for publish; your resume lives at `https://<username>.github.io/<repo>/`.

## File overview
- `index.html` — Tailwind CDN resume page with A4 print styles and your current CV format.
- `cover-letter.html` — Tailwind CDN cover letter page with matching visual style and A4 print layout.
- `data/resume.json` — Structured content powering the page (`basics`, `skills`, `soft_skills`, `languages`, `education`, `volunteering`, `references`).
- `data/cover-letter.json` — Structured content for cover letters (`basics`, `letter`).
- `resume-playbook.md` — Human-readable source content and tailoring checklist.

## Tips for tailoring
- Keep section order unchanged to preserve your current format.
- Match terminology in the job description (Finland CVs favor clarity over buzzwords).
- Keep education and volunteering bullet points short and impact-focused.
- If you need section order tweaks, adjust the DOM blocks in `index.html`.
