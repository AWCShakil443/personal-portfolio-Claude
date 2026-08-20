[README.md](https://github.com/user-attachments/files/31121271/README.md)
# Md Shakil Hossain — Portfolio Site

A single-page, self-contained portfolio site (finance / internal-audit themed) built with plain HTML + CSS + JS — no build step, no dependencies to install. Ready to publish on **GitHub Pages** in a few minutes.

## What's inside
- `index.html` — the entire site (structure, styling, and interactivity in one file, plus Google Fonts loaded via CDN)

## Publish it on GitHub Pages (free)

1. **Create a repository**
   - Go to [github.com/new](https://github.com/new)
   - Name it either:
     - `<your-username>.github.io` → site goes live at `https://<your-username>.github.io`
     - or anything else, e.g. `portfolio` → site goes live at `https://<your-username>.github.io/portfolio`
   - Set it to **Public**, then create it.

2. **Upload the file**
   - On the new repo page, click **"uploading an existing file"**
   - Drag in `index.html` (and your resume PDF if you add one — see below)
   - Commit the changes.

3. **Turn on Pages**
   - Go to **Settings → Pages** in the repo
   - Under "Build and deployment", set **Source = Deploy from a branch**
   - Branch = `main`, folder = `/ (root)` → **Save**
   - Wait 1–2 minutes, then visit the URL GitHub shows you.

That's it — no build tools, no npm install, nothing to compile.

## Optional: add a downloadable resume
1. Put a PDF version of your resume in the repo, e.g. `assets/resume.pdf`
2. In `index.html`, find:
   ```html
   <a class="btn btn-ghost" href="[#](https://drive.google.com/open?id=1BQwOAwYnruFbda47eXVyWJEHBmTwvGKT&usp=drive_fs)" id="downloadCta">Download Resume</a>
   ```
   and change `href="#"` to `href="assets/resume.pdf"` (add `download` attribute if you want it to force-download instead of opening in-browser).

## Optional: custom domain
Settings → Pages → "Custom domain" — point your domain's DNS `CNAME` record to `<your-username>.github.io` and GitHub handles the rest (free HTTPS included).

## Editing content later
Everything lives in `index.html` — search for the section you want to change:
- `#about` — summary
- `#experience` — job history ("ledger" entries)
- `#skills` — skill chips
- `#engagements` — audit engagement / client list (doubles as a "projects" section)
- `#credentials` — education & certifications
- `#contact` — email / phone / LinkedIn

## A note on LinkedIn data
I wasn't able to pull anything from your LinkedIn profile directly — public profile pages sit behind LinkedIn's login wall, so an automated fetch just returns a sign-in page, not your actual content. Everything on the site is sourced from your uploaded resumes instead. If you want your LinkedIn **articles**, **posts**, **recommendations**, or any **certifications/projects not already on your resume** included, paste that text in and I'll fold it into the relevant section.

## Design notes
- **Theme:** a "ledger" motif — deep emerald-teal background, gold accents (like an official audit stamp), tabular monospace figures for dates/results, entries numbered like ledger folios (since your work history and audit client list are genuinely sequential/categorical records — the numbering isn't decorative).
- **Type:** Fraunces (serif, headings) + Manrope (sans, body) + IBM Plex Mono (dates, figures, labels).
- **Built to hold up:** responsive down to mobile, visible keyboard focus states, respects `prefers-reduced-motion`, semantic HTML, no external JS frameworks — so it'll keep working with zero maintenance.
