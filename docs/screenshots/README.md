# Screenshot Shot List

The `.png` files in this folder are **illustrative mockups** (labeled as such in the corner of each image) standing in for the real product UI, referenced from the [README](../../README.md) and [feature walkthrough](../features.md). They're placeholders — not a claim about the actual interface.

Each mockup also has a matching `.svg` source file (same base name) — that's the editable version if you want to tweak a mockup; the `.png` is the rendered file actually linked from the docs.

## Replacing a mockup with a real screenshot

Just overwrite the `.png` file with your real screenshot/GIF, using the **same filename**. The README and feature walkthrough already point at these exact paths, so no link changes are needed. Once you're happy with it, you can delete the matching `.svg` source (no longer needed).

| Filename | Used in | What to capture |
|---|---|---|
| `qa-chat.png` | README, features.md | The Q&A interface: a natural-language question and its verified, plain-language answer |
| `verification-status.png` | features.md | A verified figure and, ideally, one flagged as unverifiable — showing both states |
| `company-report.png` | README, features.md | An automated company report (performance, peer comparison, drivers of change) |
| `peer-comparison.png` | README, features.md | A peer comparison visualization, ideally mid-drill-down into a data point |
| `admin-console.png` | README, features.md | The admin console: user/role management view |
| `audit-log.png` | features.md | The audit log viewer showing logged questions/answers/verification outcomes |
| `cost-observability.png` | README, features.md | Cost tracking dashboard: spend trend, breakdown by feature/department/user, flagged outliers |
| `agent-efficiency.png` | README, features.md | Agentic efficiency dashboard: tool-call trace with a flagged redundant call, call volume by tool |
| `rag-quality.png` | README, features.md | RAG quality dashboard: grounding rate trend, retrieval issues by category, flagged retrievals |

If your real capture is a GIF instead, name it `<filename>.gif` and update the one matching link in the README/features.md to the `.gif` extension.
