# One-page Tailwind Resume (Finland-ready)

Static, single-page resume that reads data from `data/resume.json`, prints cleanly on A4, and deploys easily to GitHub Pages.

## How to use
1) Edit your content in `resume-playbook.md` (source of truth) and mirror updates into `data/resume.json`.
2) Open `index.html` in the browser to preview. Click **Reload data** after edits to `resume.json`.
3) For each application, tailor `basics.summary`, reorder `skills`, and adjust education/volunteering bullets in `data/resume.json` to match the job description.
4) Print or save to PDF via the **Print / Save PDF** button. In the print dialog pick **A4**, scale 100%, and uncheck headers/footers.

## GitHub Pages deployment
1) Commit all files to your repo.
2) In GitHub: Settings → Pages → Build and deployment → Source = `Deploy from a branch`; Branch = `main` (or default) `/root`.
3) Wait for publish; your resume lives at `https://<username>.github.io/<repo>/`.

## File overview
- `index.html` — Tailwind CDN build with A4 print styles and a two-column format matching your CV.
- `data/resume.json` — Structured content powering the page (`basics`, `skills`, `soft_skills`, `languages`, `education`, `volunteering`, `references`).
- `resume-playbook.md` — Human-readable source content and tailoring checklist.

## Tips for tailoring
- Keep section order unchanged to preserve your current format.
- Match terminology in the job description (Finland CVs favor clarity over buzzwords).
- Keep education and volunteering bullet points short and impact-focused.
- If you need section order tweaks, adjust the DOM blocks in `index.html`.
