# The 10 & 2 Report (website)

Static site for the "10 asians and 2 white guys" fantasy league newsletter. Hosted free on GitHub Pages.
Two issues a week: Tuesday recap and Thursday Kickoff Edition (both scheduled tasks publish here automatically).

## Add a new issue
1. Make `issues/<slug>/` (e.g. `2026-week-04` or `2026-week-05-preview`) with `issue.html` (the newsletter body markup) and the PDF.
2. Add an entry to the top of `issues.json` (slug, title, date, date_label, pdf, headline, description).
3. Run `python3 build_site.py`, then commit and push. GitHub Pages redeploys in about a minute.

## Files
- `newsletter.css` – the newsletter's own styles (shared with the PDF)
- `build_site.py` – builds index.html (latest issue), issues/*/index.html, archive/, sitemap.xml, robots.txt, site.css
- `site.json` – site URL, name and header brand
