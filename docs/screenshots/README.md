# Screenshot Shot List

The `.svg` files in this folder are **illustrative mockups** (clearly labeled as such in the corner of each image) standing in for the real product UI, referenced from the [README](../../README.md) and [feature walkthrough](../features.md). They're placeholders — not a claim about the actual interface — so the "See it in action" section renders properly instead of showing broken links.

## Replacing a mockup with a real screenshot

1. Add your real screenshot/GIF to this folder, e.g. `qa-chat.png` or `qa-chat.gif`.
2. Update the matching image reference(s) in `README.md` and `docs/features.md` to point to the new filename (they currently point to the `.svg` mockup of the same base name).
3. Delete the old `.svg` mockup once it's replaced.

| Base name | Used in | What to capture |
|---|---|---|
| `qa-chat` | README, features.md | The Q&A interface: a natural-language question and its verified, plain-language answer |
| `verification-status` | features.md | A verified figure and, ideally, one flagged as unverifiable — showing both states |
| `company-report` | README, features.md | An automated company report (performance, peer comparison, drivers of change) |
| `peer-comparison` | README, features.md | A peer comparison visualization, ideally mid-drill-down into a data point |
| `admin-console` | README, features.md | The admin console: user/role management view |
| `audit-log` | features.md | The audit log viewer showing logged questions/answers/verification outcomes |

PNG or GIF both work for the real capture. Keep filenames lowercase with hyphens, matching the table above.
