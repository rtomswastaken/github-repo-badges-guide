# Pair Extraordinaire Achievement Guide

The **Pair Extraordinaire** achievement is awarded for collaborating on code through **co-authored commits** on a pull request that is merged into the default branch.

---

## Achievement Tiers

| Tier | Required Merged Co-authored Commits | Badge Preview |
| :--- | :---: | :---: |
| **Default** | 1 | <img src="../../Media/Badges/Pair-Extraordinaire/PNG/PairExtraordinaire.png" width="60"> |
| **Bronze** | 10 | <img src="../../Media/Badges/Pair-Extraordinaire/PNG/PairExtraordinaire_Bronze.png" width="60"> |
| **Silver** | 24 | <img src="../../Media/Badges/Pair-Extraordinaire/PNG/PairExtraordinaire_Silver.png" width="60"> |
| **Gold** | 48 | <img src="../../Media/Badges/Pair-Extraordinaire/PNG/PairExtraordinaire_Gold.png" width="60"> |

---

## How It Works

GitHub recognizes co-authors through the `Co-authored-by:` trailer in a Git commit message. 

When a commit containing one or more valid `Co-authored-by:` trailers is merged via a pull request into the default branch, both the commit author and all listed co-authors receive credit toward the **Pair Extraordinaire** achievement.

---

## Exact Commit Trailer Syntax

To format a co-authored commit properly:
1. Leave an empty blank line between the commit subject/body and the co-author trailer.
2. The trailer must begin with `Co-authored-by: Name <email@example.com>`.
3. Multiple co-authors must each be on their own line.

```text
Add user authentication module

Implements session handling and token validation.

Co-authored-by: Alice Developer <alice@example.com>
Co-authored-by: Bob Engineer <bob@example.com>
```

---

## Step-by-Step Walkthrough

### 1. Create a Branch
```bash
git checkout -b feature/collaborative-feature
```

### 2. Commit with Co-author Trailer
Use Git's `-m` flag with newlines, or an editor:

```bash
git commit -m "feat: implement caching layer" -m "Co-authored-by: Collaborator Name <collaborator@users.noreply.github.com>"
```

*Tip: If your collaborator wants to keep their personal email address private, they can use their GitHub-provided noreply email address found under [Email Settings](https://github.com/settings/emails).*

### 3. Push and Open a Pull Request
```bash
git push -u origin feature/collaborative-feature
gh pr create --title "feat: implement caching layer" --body "Co-authored PR"
```

### 4. Merge the Pull Request
Merge the pull request into the repository's default branch (`main`):
```bash
gh pr merge --merge --delete-branch
```

---

## Troubleshooting & Verification

- **Email Association:** The email in `Co-authored-by: Name <email>` must match an email verified on the co-author's GitHub account.
- **Squash Merges:** If you use **Squash and merge**, ensure the squash commit message preserves the `Co-authored-by:` trailers. GitHub's UI automatically pre-populates co-authors in squash commit summaries if they were in the branch commits, but always confirm the trailer is visible in the commit box before clicking confirm.
- **Rebase Merges:** Standard merge commits or rebase merges retain the original commit and trailers as-is.
