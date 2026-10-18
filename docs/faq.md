# Frequently Asked Questions & Troubleshooting

This document answers common questions regarding GitHub profile achievements, badge display settings, privacy constraints, and troubleshooting missing badges.

---

## 1. How do I show or hide achievements on my profile?

GitHub lets you globally toggle achievements or hide individual badges:

### Global Toggle:
1. Click your profile photo in the top right corner and select **Settings**.
2. In the left navigation, select **Profile** (or **Public profile**).
3. Scroll down to the **Achievements** section.
4. Check or uncheck **Show Achievements on my profile**.
5. Click **Update preferences**.

### Hiding an Individual Achievement:
1. Go to your public profile page (`https://github.com/<your-username>`).
2. In the left sidebar under **Achievements**, click on the specific badge you wish to hide.
3. Click the gear icon or **Hide achievement** option on the badge detail modal.

---

## 2. Why hasn't my badge appeared yet?

If you recently completed the unlock criteria (for example, merged a pull request or closed an issue within 5 minutes), keep the following in mind:

- **Asynchronous Processing:** GitHub processes achievements in background worker queues. Badges usually appear within 5 to 60 minutes, but high load can occasionally cause delays up to 24 hours.
- **Default Branch Requirement:** Verify that the pull request was merged into the **default branch** (`main` or `master`). Pull requests merged into secondary feature branches do not trigger achievements.
- **Account Verification:** Ensure your Git author email matches a verified email address attached to your GitHub account under [Settings > Emails](https://github.com/settings/emails).

---

## 3. How do I change the skin tone on badges?

Certain badges—specifically **Starstruck** and **Quickdraw**—feature animated emoji hands that dynamically render in 6 skin tones.

To change your emoji skin tone:
1. Navigate to [Appearance Settings](https://github.com/settings/appearance).
2. Under **Emoji skin tone preference**, select your desired tone:
   - 👋 Default (Yellow)
   - 👋🏻 Light
   - 👋🏼 Medium-Light
   - 👋🏽 Medium
   - 👋🏾 Medium-Dark
   - 👋🏿 Dark
3. Refresh your GitHub profile. The badges will update their artwork automatically.

---

## 4. Do private repository contributions count?

Yes, for achievements such as **Pull Shark** and **Pair Extraordinaire**, commits and PRs in private repositories will count if you have private contributions enabled:

1. Go to [Settings > Public Profile](https://github.com/settings/profile).
2. Under **Contribution settings**, enable **Include private contributions on my profile**.

*Note: If your entire account profile is set to Private, achievements and contributions are hidden from external visitors.*

---

## 5. Can I lose an achievement once earned?

In general, earned achievements are permanent milestones attached to your profile history.

- **Public Sponsor:** This badge requires at least one active public sponsorship. If you cancel all sponsorships, the badge may be archived or removed from the active highlights.
- **Deleted Repositories:** Deleting a repository that earned Starstruck may cause the star count calculation to re-evaluate during future platform audits, potentially affecting tier status if the qualifying stars are removed.
- **Retired Badges:** Legacy badges (Mars 2020 Contributor, Arctic Code Vault Contributor) are permanently retained by those who earned them prior to the snapshot date.
