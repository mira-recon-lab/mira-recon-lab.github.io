# MIRA Lab Website — al-folio Migration Starter Kit

This package contains the **content extracted from your existing Google Sites** (https://sites.google.com/view/mira-lab/), restructured for the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

It is a **content starter kit**, not a deployable repo. You'll merge these files into a fresh al-folio fork.

---

## What's included

```
mira-lab/
├── _config.yml                 # MIRA Lab–specific Jekyll/al-folio config
├── _bibliography/
│   └── papers.bib              # 14 journals + 2 conf. papers + ~45 abstracts
├── _pages/
│   ├── about.md                # Home page (PI intro + research topics)
│   ├── research.md             # Three research thrusts
│   ├── people.md               # PI + 5 current + 4 alumni
│   ├── publications.md         # Auto-generated from papers.bib
│   ├── software.md             # Grid of software/projects
│   └── ko-recruiting.md        # /ko/recruiting/ — Korean student notice
├── _projects/                  # One .md per software package
│   ├── 1_zero-mirid.md
│   ├── 2_wave-modl.md
│   ├── 3_wave-epi.md
│   ├── 4_vudu.md
│   ├── 5_vudu-sage.md
│   └── 6_gslider-buda.md
├── _news/                      # Empty — ready for future announcements
└── README.md                   # This file
```

---

## Setup steps

### 1. Fork al-folio

Go to https://github.com/alshedivat/al-folio and click **Use this template**. Name the repo either:

- `<your-username>.github.io` — for a user/organization site at `https://<username>.github.io`, or
- `mira-lab` — for a project site at `https://<username>.github.io/mira-lab/`

### 2. Clone and merge this starter content

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# Copy the starter files over (overwrites defaults — back up if needed)
cp -r /path/to/mira-lab/_bibliography .
cp -r /path/to/mira-lab/_pages .
cp -r /path/to/mira-lab/_projects .
cp /path/to/mira-lab/_config.yml .
```

### 3. Update `_config.yml`

Edit these fields in `_config.yml`:

- `url:` → `https://<your-username>.github.io`
- `baseurl:` → leave blank for user site; set to `/mira-lab` for project site
- `github_username:` → your GitHub handle
- `scholar_userid:` → your Google Scholar ID
- `linkedin_username:`, `twitter_username:`, etc. → as desired

### 4. Add images

Place these images in `assets/img/`:

| File                     | What it is                 | Where to source                                       |
| ------------------------ | -------------------------- | ----------------------------------------------------- |
| `prof_pic.jpg`           | PI profile photo           | Use the photo from Google Sites or upload a new one   |
| `research_wave_modl.jpg` | Deep learning recon figure | From Google Sites Research page                       |
| `research_qmri.jpg`      | Quantitative MRI figure    | From Google Sites Research page                       |
| `research_dmri.jpg`      | Diffusion MRI figure       | From Google Sites Research page                       |
| `software_*.jpg`         | Software thumbnails        | Optional — use a generic placeholder if not available |

**Tip:** Right-click → "Save image as" on each figure from your Google Sites page, then drop them into `assets/img/`.

### 5. Test locally (optional but recommended)

```bash
bundle install
bundle exec jekyll serve
# Open http://localhost:4000
```

### 6. Deploy

Push to GitHub. al-folio includes a GitHub Actions workflow that builds and deploys automatically.

```bash
git add .
git commit -m "Initial MIRA Lab site content"
git push origin main
```

Then in your repo settings → **Pages** → set source to **GitHub Actions**.

---

## Notes on the migrated content

### Publications

All publications in `papers.bib` use the following custom al-folio fields:

- `abbr` — journal/conference badge (MRM, ISMRM, MICCAI, etc.)
- `selected: true` — marks 6 first-author papers to highlight on the homepage
- `award` / `award_name` — ISMRM Merit Awards, Editor's Pick
- `code` — GitHub repo links
- `arxiv` — arXiv preprint IDs
- `doi` / `url` — DOI links

To **add a new paper later**, just append a new BibTeX entry to `_bibliography/papers.bib`. Claude can do this for you in seconds — paste the bibliography from the publisher and ask Claude to convert it.

### Members

Names are kept in **Hangul (Korean)** as you requested. If you later collect English transliterations, edit `_pages/people.md`.

### Korean recruiting page

Lives at `/ko/recruiting/`. The English home page links to it. To remove the link from the English navbar but keep the page accessible by direct URL, the `nav: false` flag in the page's front matter already handles this.

### Software grid

The `/software/` page renders a card grid using al-folio's projects collection, split into two categories: **Open Source** and **Customer-to-Producer**.

---

## What you'll want to do soon

- [ ] Replace `assets/img/prof_pic.jpg` with your actual profile photo
- [ ] Add the three research figures (download from Google Sites)
- [ ] Optionally add thumbnail images for the software grid
- [ ] Fill in `_config.yml` with your GitHub/Scholar/etc. handles
- [ ] Add a CNAME if you have a custom domain (e.g. `miralab.sejong.ac.kr`)
- [ ] Put the Google Sites homepage into "transition notice" mode pointing to the new URL

---

Generated by Claude based on content from https://sites.google.com/view/mira-lab/
