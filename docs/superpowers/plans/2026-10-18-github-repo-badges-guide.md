# GitHub Repo Badges Guide Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create and publish `rtomswastaken/github-repo-badges-guide`, an authoritative, beautifully formatted reference and step-by-step tutorial guide for earning all GitHub achievements, profile highlights, and badges.

**Architecture:** A comprehensive single-page master dashboard (`README.md`) following the Goated README standard paired with dedicated deep-dive sub-documents (`docs/achievements/*.md`, `docs/highlights/*.md`, `docs/faq.md`) and self-contained high-resolution local media assets (`Media/`).

**Tech Stack:** Markdown, Git, GitHub CLI (`gh`), SVG/PNG media assets.

**Spec:** `docs/superpowers/specs/2026-10-18-github-repo-badges-guide-design.md`

## Global Constraints

- Grounded strictly in real, verified GitHub platform behavior and current tier metrics.
- Adhere to the Goated README philosophy: clear headers, exact tables, zero promotional hype, copy-pasteable Git commands.
- All media references must resolve to local files within `Media/`.
- Cross-document links must use valid relative Markdown links.
- License must be standard MIT licensed to `rtomswastaken`.

---

### Task 1: Scaffolding, Licensing, and Asset Verification

**Files:**
- Create: `LICENSE`
- Modify: `.gitattributes`
- Test: Verify directory tree and files with shell commands

**Interfaces:**
- Produces: Base repository structure, MIT license, and validated `Media/` asset directory.

- [ ] **Step 1: Create MIT LICENSE file**
Write `LICENSE` with standard MIT terms under `rtomswastaken`.

- [ ] **Step 2: Verify and configure .gitattributes**
Ensure Git LFS or binary tracking is properly configured for PNG and SVG images.

- [ ] **Step 3: Run asset presence test**
Verify all required PNG and SVG directories exist under `Media/Badges` and `Media/Highlights`.

- [ ] **Step 4: Commit scaffolding**
```bash
git add LICENSE .gitattributes Media/ docs/superpowers/
git commit -m "chore: scaffold repo structure, license, and assets"
```

---

### Task 2: Active Achievement Step-by-Step Tutorials

**Files:**
- Create: `docs/achievements/pull-shark.md`
- Create: `docs/achievements/galaxy-brain.md`
- Create: `docs/achievements/yolo.md`
- Create: `docs/achievements/quickdraw.md`
- Create: `docs/achievements/pair-extraordinaire.md`
- Create: `docs/achievements/starstruck.md`
- Create: `docs/achievements/public-sponsor.md`

**Interfaces:**
- Consumes: Tier metrics from `docs/superpowers/specs/2026-10-18-github-repo-badges-guide-design.md`.
- Produces: In-depth guides referenced by `README.md`.

- [ ] **Step 1: Write pull-shark.md**
Detailed guide for Pull Shark: requirements (2, 16, 128, 1024 PRs), branch strategy, PR merging rules, why self-merged PRs qualify, and troubleshooting.

- [ ] **Step 2: Write galaxy-brain.md**
Detailed guide for Galaxy Brain: finding discussions, providing accepted answers (2, 8, 16, 32), community guidelines, and common pitfalls.

- [ ] **Step 3: Write yolo.md**
Detailed guide for YOLO: merging a PR without a review, handling repo settings/branch protection rules, and single-author repo tips.

- [ ] **Step 4: Write quickdraw.md**
Detailed guide for Quickdraw: creating an issue or PR and closing it within 5 minutes, shell/CLI quick command walkthrough.

- [ ] **Step 5: Write pair-extraordinaire.md**
Detailed guide for Pair Extraordinaire: exact `Co-authored-by:` syntax (name and email), multiple co-authors, Git commit trailer formatting, and tiers (1, 10, 24, 48).

- [ ] **Step 6: Write starstruck.md**
Detailed guide for Starstruck: repository stardom milestones (16, 128, 512, 4096), genuine ways to showcase projects, and skin tone interactions.

- [ ] **Step 7: Write public-sponsor.md**
Detailed guide for Public Sponsor: GitHub Sponsors program, setting up sponsorship, making sponsorship public vs. private, and tiers.

- [ ] **Step 8: Verify file creation and relative links**
Run test script to verify all 7 achievement docs exist and contain non-empty content.

- [ ] **Step 9: Commit achievement guides**
```bash
git add docs/achievements/
git commit -m "docs: add comprehensive tutorials for all active achievements"
```

---

### Task 3: Highlights & FAQ Documentation

**Files:**
- Create: `docs/highlights/profile-highlights.md`
- Create: `docs/faq.md`

**Interfaces:**
- Consumes: GitHub status programs and community FAQ criteria.
- Produces: Supporting reference pages for `README.md`.

- [ ] **Step 1: Write profile-highlights.md**
Covers GitHub Pro, Developer Program Member, Security Bug Bounty Hunter, GitHub Campus Expert, and Security Advisory Credit, with official application URLs and prerequisite criteria.

- [ ] **Step 2: Write faq.md**
Addresses how to show/hide badges, skin tone customization, private profile restrictions, sync and cache delays, and how badge updates propagate.

- [ ] **Step 3: Commit highlights and FAQ documentation**
```bash
git add docs/highlights/ docs/faq.md
git commit -m "docs: add profile highlights and achievement FAQ guides"
```

---

### Task 4: Master Dashboard (README.md)

**Files:**
- Create: `README.md`

**Interfaces:**
- Consumes: Assets from `Media/`, guides from `docs/`, and spec from `docs/superpowers/specs/2026-10-18-github-repo-badges-guide-design.md`.
- Produces: The primary repository README adhering to Goated README standards.

- [ ] **Step 1: Author README.md header & quick navigation**
Project title, clean description, and categorized table of contents.

- [ ] **Step 2: Author Active Achievements table**
Formatted table with columns: Badge preview, Name, Requirement description, Tier table with embedded local images and counts, and link to step-by-step guide.

- [ ] **Step 3: Author Emoji Skin Tone Variations section**
Visual comparison table showing Starstruck and Quickdraw across all 6 skin tones with instructions on how to switch tone in settings.

- [ ] **Step 4: Author Profile Highlights section**
Table supporting dark/light mode SVGs (`#gh-dark-mode-only` and `#gh-light-mode-only`) for each highlight badge with links to `docs/highlights/profile-highlights.md`.

- [ ] **Step 5: Author Retired Badges and Experimental Badges sections**
Mars 2020 Contributor, Arctic Code Vault Contributor, Heart on Your Sleeve, and Open Sourcerer with historical documentation.

- [ ] **Step 6: Author Profile Configuration & FAQ summary**
Brief configuration instructions linking to `docs/faq.md` and MIT License attribution.

- [ ] **Step 7: Verify README rendering and link integrity**
Check all local asset paths and relative links referenced in `README.md`.

- [ ] **Step 8: Commit README.md**
```bash
git add README.md
git commit -m "docs: create comprehensive goated achievements README dashboard"
```

---

### Task 5: Publication to GitHub

**Files:**
- Modify: git remote configuration

**Interfaces:**
- Consumes: Local git repository `github-repo-badges-guide`.
- Produces: Live public repository `https://github.com/rtomswastaken/github-repo-badges-guide`.

- [ ] **Step 1: Create public GitHub repository via gh CLI**
```bash
gh repo create rtomswastaken/github-repo-badges-guide --public --source=. --description="Definitive visual guide and step-by-step tutorials for unlocking all GitHub achievements, profile badges, and highlights." --push
```

- [ ] **Step 2: Verify remote repository on GitHub**
Verify repository page and commits via `gh repo view rtomswastaken/github-repo-badges-guide`.
