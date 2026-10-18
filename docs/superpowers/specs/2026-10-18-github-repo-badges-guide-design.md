# GitHub Repo Badges & Achievements Guide - Design Specification

**Date:** 2026-10-18  
**Repository:** `rtomswastaken/github-repo-badges-guide`  
**Status:** Approved  

---

## 1. Overview & Objective

The objective of this repository is to provide the definitive, accurate, and cleanly structured guide for earning and displaying every GitHub profile achievement, highlight, and legacy badge.

Unlike existing outdated or cluttered badge lists, this repository follows the **Goated README** philosophy:
- Grounded strictly in verified GitHub platform mechanics and documentation.
- Crisp, self-contained visual catalogs featuring local high-res SVG/PNG assets.
- Clean separation between the main dashboard (`README.md`) and dedicated, deep-dive walkthroughs (`docs/achievements/*.md`).
- Free of marketing fluff, generic AI filler, and broken links.

---

## 2. Architecture & File Structure

```text
github-repo-badges-guide/
├── README.md                          # Primary reference dashboard & visual catalog
├── LICENSE                            # MIT License
├── .gitattributes                     # Asset handling rules
├── Media/                             # Self-contained visual assets
│   ├── Badges/                        # Active, experimental, and retired badges (PNG/SVG)
│   │   ├── Pull-Shark/
│   │   ├── Galaxy-Brain/
│   │   ├── YOLO/
│   │   ├── Quick-Draw/
│   │   ├── Pair-Extraordinaire/
│   │   ├── Star-Struck/
│   │   ├── GitHub-Sponsor/
│   │   ├── Heart-on-your-sleeve/      # Experimental / unreleased
│   │   ├── Open-Sourcerer/            # Experimental / unreleased
│   │   ├── Mars-2020-Contributor/     # Retired
│   │   └── 2020-Arctic-Code-Vault/    # Retired
│   └── Highlights/                    # Status badges (Dark/Light SVG variations)
│       ├── GitHub-Pro/
│       ├── Developer-Program-Member/
│       ├── GitHub-Campus-Expert/
│       ├── Security-Advisory-Credit/
│       └── Security-Bug-Bounty-Hunter/
└── docs/
    ├── achievements/                  # Deep-dive tutorials per achievement
    │   ├── pull-shark.md
    │   ├── galaxy-brain.md
    │   ├── yolo.md
    │   ├── quickdraw.md
    │   ├── pair-extraordinaire.md
    │   ├── starstruck.md
    │   └── public-sponsor.md
    ├── highlights/
    │   └── profile-highlights.md      # Criteria & applications for highlights
    └── faq.md                         # Visibility toggles, delay in distribution, troubleshooting
```

---

## 3. Verified Achievement Specifications

### 3.1 Active Achievements & Exact Tiers

| Badge | Achievement Name | Unlock Criteria | Tiers (Requirements) |
| :--- | :--- | :--- | :--- |
| **Pull Shark** | Pull Shark | Open a pull request that gets merged into default branch | Default: 2 PRs<br>Bronze: 16 PRs<br>Silver: 128 PRs<br>Gold: 1,024 PRs |
| **Galaxy Brain** | Galaxy Brain | Have answers accepted in GitHub Discussions | Default: 2 answers<br>Bronze: 8 answers<br>Silver: 16 answers<br>Gold: 32 answers |
| **YOLO** | YOLO | Merge a pull request without receiving a code review | Default: 1 PR |
| **Quickdraw** | Quickdraw | Close an issue or PR within 5 minutes of opening | Default: 1 issue/PR |
| **Pair Extraordinaire** | Pair Extraordinaire | Co-author commits on a merged pull request | Default: 1 commit<br>Bronze: 10 commits<br>Silver: 24 commits<br>Gold: 48 commits |
| **Starstruck** | Starstruck | Create repository(ies) that reach star milestones | Default: 16 stars<br>Bronze: 128 stars<br>Silver: 512 stars<br>Gold: 4,096 stars |
| **Public Sponsor** | Public Sponsor | Sponsor an open-source contributor via GitHub Sponsors | Default: 1 active sponsorship |

### 3.2 Skin Tone Variations
- **Starstruck** and **Quickdraw** adjust visual appearance according to the user's Emoji Skin Tone Preference selected at `https://github.com/settings/appearance`.
- 6 variants: Standard (Default 👋), Light (👋🏻), Medium-Light (👋🏼), Medium (👋🏽), Medium-Dark (👋🏾), Dark (👋🏿).

### 3.3 Profile Highlights (Status Badges)
- **GitHub Pro:** Active GitHub Pro subscription.
- **Developer Program Member:** Registered member of the GitHub Developer Program.
- **Security Bug Bounty Hunter:** Valid vulnerability reported through GitHub Security Bug Bounty program.
- **GitHub Campus Expert:** Completed the GitHub Campus Experts training program.
- **Security Advisory Credit:** Author or contributor credited in an advisory accepted into the GitHub Advisory Database.

### 3.4 Retired / Legacy Badges (No Longer Earnable)
- **Mars 2020 Contributor:** Contributed code to repositories used by NASA JPL in the Mars 2020 Helicopter Mission (Ingenuity).
- **Arctic Code Vault Contributor:** Contributed code to repositories archived in the Arctic Code Vault snapshot in Feb 2020.

### 3.5 Experimental / Unreleased Badges
- **Open Sourcerer:** Experimental badge designed for PR merges across independent public repositories.
- **Heart on Your Sleeve:** Experimental badge historically tested with ❤️ reactions.

---

## 4. Documentation Standards

Following `goated-readme`:
- Accurate tables with explicit image widths (`60px`) and centered alignments.
- Direct links to official GitHub settings, documentation, and dedicated tutorial sub-documents.
- No artificial fluff or promotional text.
- Tested and copy-pasteable Git CLI commands for co-authoring, PR merging, and issue management.
