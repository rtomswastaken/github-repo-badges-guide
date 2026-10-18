# YOLO Achievement Guide

The **YOLO** achievement is unlocked when you merge a pull request without waiting for or receiving a code review.

---

## Achievement Tier

| Tier | Required Merged Pull Requests | Badge Preview |
| :--- | :---: | :---: |
| **Default** | 1 | <img src="../../Media/Badges/YOLO/PNG/YOLO_Badge.png" width="60"> |

*Note: YOLO is a single-tier achievement with no Bronze, Silver, or Gold variants.*

---

## How It Works

GitHub checks the review status of a pull request at the moment it is merged:
1. You open a pull request.
2. The pull request has zero approved or pending review submissions from other reviewers.
3. You immediately merge the pull request into the default branch.

Because repository owners have direct write access and can merge without reviews on unrestricted branches, this achievement is one of the quickest to unlock on any personal repository.

---

## Step-by-Step Guide

### 1. Ensure Branch Protection Does Not Require Reviews
In a personal repository:
1. Navigate to **Settings** > **Branches**.
2. If branch protection rules exist for `main`, ensure **Require a pull request before merging** > **Require approvals** is unchecked (or disabled temporarily).

### 2. Create and Push a Branch
```bash
git checkout -b patch/quick-fix
echo "export const VERSION = '1.0.1';" >> version.js
git add version.js
git commit -m "fix: bump version"
git push -u origin patch/quick-fix
```

### 3. Open and Merge Immediately (No Reviews)
Using GitHub CLI:
```bash
gh pr create --title "fix: quick version bump" --body "Direct merge without code review."
gh pr merge --merge --delete-branch
```

Or via GitHub web:
1. Click **Compare & pull request**.
2. Click **Create pull request**.
3. Do **not** request reviewers or submit a review.
4. Directly click **Merge pull request** and confirm.

---

## Verification

Once merged, GitHub queues the achievement calculation. Check your profile (`https://github.com/<your-username>`) after 5 to 15 minutes.
