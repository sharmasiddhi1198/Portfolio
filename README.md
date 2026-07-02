# Siddhi Sharma — Portfolio (GenAI Consultant & Automation Engineer)

A 4-page personal portfolio site (About, Resume, Projects, Contact), built as
plain HTML/CSS/JS — no build step, works directly with GitHub Pages.

## Files
```
index.html      → About page
resume.html     → Resume (timeline + skills + certifications)
projects.html   → Case studies (BriefAI, Amazon BI work, A/B test project)
contact.html    → Contact links
assets/
  style.css     → All styling (design tokens at the top)
  script.js     → Mobile nav toggle + scroll-reveal animation
  Siddhi_Sharma_Resume.pdf → Downloadable CV (linked from resume.html)
```

## Before you publish — fill these in
Search each HTML file for these placeholders and replace with your real links:
- `https://www.linkedin.com/in/` → your actual LinkedIn profile URL
- `https://github.com/sharmasiddhi1198` → confirm this is your GitHub username (used throughout)

Also consider:
- Add a headshot/photo — drop an image into `assets/` and reference it in the
  hero section of `index.html` if you want one (the current design works
  fine without a photo too).
- Swap `assets/Siddhi_Sharma_Resume.pdf` for whichever resume version you
  want as your default downloadable CV.

## Deploy with GitHub Pages (two options)

### Option A — Personal site (yourusername.github.io)
1. Create a new GitHub repo named exactly `sharmasiddhi1198.github.io`
   (must match your GitHub username exactly).
2. Upload all files in this folder to the root of that repo (keep the
   `assets/` folder structure intact).
3. Go to the repo's **Settings → Pages**. It should auto-detect and deploy
   from the `main` branch, root folder.
4. Your site will be live at `https://sharmasiddhi1198.github.io/` within a
   few minutes.

### Option B — Project site (any repo name, e.g. `portfolio`)
1. Create a new repo, e.g. `portfolio`.
2. Upload all files here to the root of that repo.
3. Go to **Settings → Pages** → under "Build and deployment," set
   **Source: Deploy from a branch**, branch: `main`, folder: `/ (root)`.
4. Your site will be live at `https://sharmasiddhi1198.github.io/portfolio/`.

Either way, no build tools, npm, or GitHub Actions are required — GitHub
Pages serves the static files directly.

## Updating content later
- Resume timeline, skills, and certifications: edit `resume.html` directly.
- Add a new case study: copy one `.case-study` block in `projects.html` and
  edit the text/tags.
- Colors and fonts: all defined as CSS variables at the top of
  `assets/style.css` under `:root`.
